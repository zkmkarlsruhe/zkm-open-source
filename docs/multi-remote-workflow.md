# Multi-Remote Git Workflows

Guide for managing projects across multiple Git remotes (GitHub, GitLab, etc.).

---

## Option 1: Mirror Setup (Same Branches Everywhere)

For projects where GitHub and GitLab should be identical mirrors.

### Setup

```bash
# Add both remotes
git remote add github git@github.com:zkmkarlsruhe/PROJECT.git
git remote add gitlab git@git.zkm.de:GROUP/PROJECT.git

# Create a remote group for pushing to both
git remote add all git@github.com:zkmkarlsruhe/PROJECT.git
git remote set-url --add --push all git@github.com:zkmkarlsruhe/PROJECT.git
git remote set-url --add --push all git@git.zkm.de:GROUP/PROJECT.git
```

### Daily Use

```bash
# Push to both remotes at once
git push all main

# Or push with tags
git push all main --tags
```

### Verify Setup

```bash
git remote -v
# Should show:
# all     git@github.com:zkmkarlsruhe/PROJECT.git (fetch)
# all     git@github.com:zkmkarlsruhe/PROJECT.git (push)
# all     git@git.zkm.de:GROUP/PROJECT.git (push)
```

### Git Alias (Optional)

Add to `~/.gitconfig`:

```ini
[alias]
    pushall = !git push github && git push gitlab
```

Then use: `git pushall main`

---

## Option 2: Private Dev / Public Release

For projects with private development and clean public releases.

### Architecture

```
PRIVATE (development)              PUBLIC (releases)
─────────────────────              ─────────────────

origin/dev                         main
├── all development work           ├── release commits only
├── internal docs                  ├── NO private files
├── WIP commits                    └── clean, linear history
│                                          ▲
│         squash-merge                     │
│         (exclude private dirs)           │
└──────────────────────────────────────────┘
```

### Setup

```bash
# Private development server (your main repo)
git remote add origin git@git.zkm.de:GROUP/PROJECT.git

# Public mirrors
git remote add github git@github.com:zkmkarlsruhe/PROJECT.git
```

### Branch Structure

```bash
# main branch exists on all remotes (public releases)
git checkout main
git push origin main
git push github main

# dev branch exists only on private origin
git checkout -b dev
git push origin dev
```

### Private vs Public Files

**Private (never published):**
- `devdocs/` – Internal documentation, planning, drafts
- `presentation/` – Slides, demos, talk materials
- `.internal/` – Development configuration, secrets templates

**Public (included in releases):**
- `src/` – Source code
- `docs/` – User-facing documentation
- `README.md`, `CHANGELOG.md`, `LICENSE`

### Daily Development

```bash
git checkout dev
git add .
git commit -m "feat: add new feature"
git push origin dev  # Private only
```

### Release Process

```bash
# 1. Switch to main
git checkout main

# 2. Squash-merge dev
git merge --squash dev

# 3. Exclude private directories
git reset HEAD devdocs/ presentation/ .internal/
rm -rf devdocs/ presentation/ .internal/

# 4. Commit release
git commit -m "Release vX.Y.Z"

# 5. Push to all remotes
git push origin main
git push github main

# 6. Rebase dev on main
git checkout dev
git rebase main
git push origin dev --force
```

### Handling External PRs

```bash
# 1. Merge PR on GitHub
gh pr merge 123 --squash

# 2. Sync back
git fetch github main
git checkout main
git reset --hard github/main
git push origin main

# 3. Rebase dev
git checkout dev
git rebase main
git push origin dev --force
```

---

## Branch Rules Summary

| Setup | Branch | Remotes | Force Push? |
|-------|--------|---------|-------------|
| Mirror | `main` | all | Never |
| Mirror | `dev` | all | After rebase |
| Private/Public | `dev` | origin only | After rebase |
| Private/Public | `main` | all | Never on public |

---

## Troubleshooting

### SSH Host Keys

```bash
ssh-keyscan github.com >> ~/.ssh/known_hosts
ssh-keyscan git.zkm.de >> ~/.ssh/known_hosts
```

### Verify Sync

```bash
# Check all remotes are on same commit
git rev-parse github/main origin/main
```

### Check Remote Configuration

```bash
git remote -v
git fetch --all
git branch -vv
```
