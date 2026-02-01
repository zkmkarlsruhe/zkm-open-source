# Badge Reference

Copy-paste badges for ZKM projects.

---

## "Funded by" Section (with Logo)

Place this at the **bottom** of your README, after License/Acknowledgments. The logo automatically switches between dark and light versions based on the user's color scheme preference.

```markdown
## Funded by

<p align="center">
  <a href="https://zkm.de">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/zkmkarlsruhe/zkm-open-source/main/assets/zkm-logo-light.svg">
      <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/zkmkarlsruhe/zkm-open-source/main/assets/zkm-logo.svg">
      <img alt="ZKM" src="https://raw.githubusercontent.com/zkmkarlsruhe/zkm-open-source/main/assets/zkm-logo.svg" width="120">
    </picture>
  </a>
</p>
```

### GitLab Version

```markdown
## Funded by

<p align="center">
  <a href="https://zkm.de">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://git.zkm.de/zkm-open-source/-/raw/main/assets/zkm-logo-light.svg">
      <source media="(prefers-color-scheme: light)" srcset="https://git.zkm.de/zkm-open-source/-/raw/main/assets/zkm-logo.svg">
      <img alt="ZKM" src="https://git.zkm.de/zkm-open-source/-/raw/main/assets/zkm-logo.svg" width="120">
    </picture>
  </a>
</p>
```

### Simple (No Dark Mode)

```markdown
## Funded by

[![ZKM](https://raw.githubusercontent.com/zkmkarlsruhe/zkm-open-source/main/assets/zkm-logo.svg)](https://zkm.de)
```

---

## Organization Badge

```markdown
[![ZKM](https://img.shields.io/badge/ZKM-Karlsruhe-blue)](https://zkm.de)
```

---

## Licenses

```markdown
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![License: BSD](https://img.shields.io/badge/License-BSD-blue.svg)](LICENSE)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE)
[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](LICENSE)
```

---

## Technologies

```markdown
[![openFrameworks](https://img.shields.io/badge/openFrameworks-addon-pink)](https://openframeworks.cc/)
[![Python](https://img.shields.io/badge/Python-3.x-blue)](https://python.org)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)](https://tensorflow.org)
[![Pure Data](https://img.shields.io/badge/Pure%20Data-patch-lightblue)](https://puredata.info/)
```

---

## Status

```markdown
[![Status: Active](https://img.shields.io/badge/Status-Active-success)]()
[![Status: Maintenance](https://img.shields.io/badge/Status-Maintenance-yellow)]()
[![Status: Archived](https://img.shields.io/badge/Status-Archived-lightgrey)]()
```

---

## Complete README Example

```markdown
# Project Name

[![ZKM](https://img.shields.io/badge/ZKM-Karlsruhe-blue)](https://zkm.de)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> One-line description

Part of [ZKM Open Source](https://github.com/zkmkarlsruhe)

---

## Features
...

---

## License

MIT License - see [LICENSE](LICENSE)

---

## Funded by

<p align="center">
  <a href="https://zkm.de">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/zkmkarlsruhe/zkm-open-source/main/assets/zkm-logo-light.svg">
      <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/zkmkarlsruhe/zkm-open-source/main/assets/zkm-logo.svg">
      <img alt="ZKM" src="https://raw.githubusercontent.com/zkmkarlsruhe/zkm-open-source/main/assets/zkm-logo.svg" width="120">
    </picture>
  </a>
</p>

Copyright (c) 2026 ZKM | Karlsruhe
```
