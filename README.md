<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/zkm-logo-light.svg">
    <source media="(prefers-color-scheme: light)" srcset="assets/zkm-logo.svg">
    <img alt="ZKM" src="assets/zkm-logo.svg" width="200">
  </picture>
</p>

<h1 align="center">ZKM Open Source</h1>

<p align="center">
  <a href="https://zkm.de"><img src="https://img.shields.io/badge/ZKM-Karlsruhe-blue" alt="ZKM"></a>
  <a href="https://publiccode.eu"><img src="https://img.shields.io/badge/Public%20Money-Public%20Code-blue" alt="Public Money Public Code"></a>
</p>

<p align="center">
  <strong>Open source tools and research from ZKM | Center for Art and Media Karlsruhe</strong>
</p>

<p align="center">
  <a href="https://en.wikipedia.org/wiki/ZKM_Center_for_Art_and_Media_Karlsruhe">Wikipedia</a> ·
  <a href="https://www.instagram.com/zkmkarlsruhe/">Instagram</a> ·
  <a href="https://www.youtube.com/user/ZKMkarlsruhe">YouTube</a> ·
  <a href="https://www.linkedin.com/company/zkm-zentrum-f%C3%BCr-kunst-und-medien">LinkedIn</a> ·
  <a href="https://www.facebook.com/zkmkarlsruhe">Facebook</a>
</p>

---

## About ZKM

The **ZKM | Center for Art and Media Karlsruhe** is a cultural institution founded in 1989 in Karlsruhe, Germany. It is one of the world's largest centers for media art, combining a museum, research institute, and production facility under one roof.

ZKM explores the intersection of art, science, and technology — preserving digital art, developing new forms of artistic expression, and researching the impact of media on society.

## Why Open Source?

ZKM is publicly funded by the State of Baden-Württemberg and the City of Karlsruhe. We believe in **Public Money, Public Code** — software developed with public funds should be publicly available.

By open sourcing our tools, we:
- Share knowledge with the cultural and research community
- Enable other institutions to build on our work
- Ensure transparency in publicly funded development
- Contribute back to the open source ecosystem we rely on

---

## Projects

**Platforms:** [GitHub](https://github.com/zkmkarlsruhe) (public releases) | [GitLab](https://git.zkm.de) (development)

## Quick Links

- [AI & Machine Learning](#ai--machine-learning)
- [Exhibition Infrastructure](#exhibition-infrastructure)
- [Sensors & Hardware](#sensors--hardware)
- [Audio & Spatialization](#audio--spatialization)
- [Networking & Infrastructure](#networking--infrastructure)
- [Developer Tools](#developer-tools)
- [Templates](#templates)

---

## AI & Machine Learning

Core libraries and applications for AI/ML in creative contexts.

| Project | Stars | Description |
|---------|-------|-------------|
| [**HandTracker**](https://github.com/zkmkarlsruhe/HandTracker) | 6 | Hand tracking using ofxTensorFlow2. |
| [**language-identification**](https://github.com/zkmkarlsruhe/language-identification) | 41 | Spoken language detection using deep learning. |
| [**LanguageIdentifier**](https://github.com/zkmkarlsruhe/LanguageIdentifier) | 1 | Language identification app (openFrameworks). |
| [**ofxTensorFlow2**](https://github.com/zkmkarlsruhe/ofxTensorFlow2) | 119 | TensorFlow 2 wrapper for openFrameworks. |
| [**Styler**](https://github.com/zkmkarlsruhe/Styler) | 6 | Neural style transfer for images, video, and camera. |
| [**YoloOSC**](https://github.com/zkmkarlsruhe/YoloOSC) | 22 | Real-time YOLO object detection with OSC output. |

### REST APIs (GitLab)

| Project | Description |
|---------|-------------|
| [Automatic Speech Recognition](https://git.zkm.de/Hertz-Lab/Research/intelligent-museum/automatic-speech-recognition) | Speech-to-text transcription API. |
| [Detoxify REST API](https://git.zkm.de/Hertz-Lab/Research/intelligent-museum/detoxify-rest-api) | Text toxicity detection API. |
| [Stable Diffusion API](https://git.zkm.de/Hertz-Lab/Research/intelligent-museum/stable-diffusion-api) | REST API for Stable Diffusion image generation. |

---

## Exhibition Infrastructure

Tools for running exhibitions, managing displays, and visitor interaction.

| Project | Stars | Description |
|---------|-------|-------------|
| [**baton**](https://github.com/zkmkarlsruhe/baton) | 4 | UDP/WebSocket message relay. |
| [**exhibition-vm-controller**](https://github.com/zkmkarlsruhe/exhibition-vm-controller) | - | VM management for digital art conservation. |
| [**filterdns**](https://github.com/zkmkarlsruhe/filterdns) | - | Self-hosted DNS filtering with per-profile config. |
| [**filterdns-client**](https://github.com/zkmkarlsruhe/filterdns-client) | - | Desktop client for FilterDNS (Linux/macOS/Windows). |
| [**museum-label**](https://github.com/zkmkarlsruhe/museum-label) | 2 | Auto-adaptive multilingual museum labels. |
| [**serial-button-osc**](https://github.com/zkmkarlsruhe/serial-button-osc) | 3 | Physical button → OSC messages. |
| [**thoscy**](https://github.com/zkmkarlsruhe/thoscy) | 3 | Thingsboard to OSC relay. |
| [**wayback-cache-proxy**](https://github.com/zkmkarlsruhe/wayback-cache-proxy) | 1 | Caching Wayback Machine proxy for museum exhibitions. |

### GitLab Projects

| Project | Description |
|---------|-------------|
| [Generic Exhibition Platform](https://git.zkm.de/Hertz-Lab/beyond-matter/generic-exhibition-platform) | Reusable digital exhibition framework. |
| [intelligent-things](https://git.zkm.de/Hertz-Lab/Research/intelligent-museum/intelligent-things) | IoT data system using MQTT. |
| [skeeter](https://git.zkm.de/Hertz-Lab/Research/intelligent-museum/skeeter) | MQTT ↔ OSC bridge. |


---

## Sensors & Hardware

Hardware interfaces and sensor processing tools.

| Project | Stars | Description |
|---------|-------|-------------|
| [**lidar**](https://github.com/zkmkarlsruhe/lidar) | 7 | LIDAR processing tools for spatial detection. |
| [**SOMA-Junction**](https://github.com/zkmkarlsruhe/SOMA-Junction) | - | Junction box for SOMA lighting (hardware). |
| [**stingyraycontrol9000**](https://github.com/zkmkarlsruhe/stingyraycontrol9000) | - | Cascadable LED driver for art installations (hardware). |
| [**tfluna**](https://github.com/zkmkarlsruhe/tfluna) | 3 | TF-Luna LIDAR sensor → OSC/UDP/Thingsboard. |

---

## Audio & Spatialization

3D audio rendering and spatial sound tools.

| Project | Stars | Description |
|---------|-------|-------------|
| [**ZirkoniumSpatializationServer**](https://github.com/zkmkarlsruhe/ZirkoniumSpatializationServer) | 6 | Core Zirkonium 3D audio rendering in Pure Data. |

---

## Networking & Infrastructure

Network tools and infrastructure components.

| Project | Stars | Description |
|---------|-------|-------------|
| [**arklet**](https://github.com/zkmkarlsruhe/arklet) | - | ARK identifier minter/binder/resolver. |
| [**prep-pi**](https://github.com/zkmkarlsruhe/prep-pi) | - | Raspberry Pi offline web server. |

---

## Developer Tools

Utilities for macOS packaging, CI/CD, and development workflows.

| Project | Stars | Description |
|---------|-------|-------------|
| [**js-Gerstner-wave**](https://github.com/zkmkarlsruhe/js-Gerstner-wave) | 1 | Interactive Gerstner wave simulation. |
| [**mac-dist-helper**](https://github.com/zkmkarlsruhe/mac-dist-helper) | 10 | macOS app packaging, code signing, and notarization. |
| [**mac-dist-helper-examples**](https://github.com/zkmkarlsruhe/mac-dist-helper-examples) | 2 | Example projects for mac-dist-helper. |

### GitLab Templates

| Project | Description |
|---------|-------------|
| [web-interface](https://git.zkm.de/Hertz-Lab/Research/intelligent-museum/web-interface) | HTML/Flask web UI template. |
| [p5js-template](https://git.zkm.de/Hertz-Lab/Research/intelligent-museum/p5js-template) | p5.js browser project template. |

---

## Archived / Historical

| Project | Description |
|---------|-------------|
| [bias-workshop](https://github.com/zkmkarlsruhe/bias-workshop) | Workshop materials (2021). |
| [cppflow](https://github.com/zkmkarlsruhe/cppflow) | Fork: TensorFlow C++ (use upstream). |
| [NextcloudVideo_Converter](https://github.com/zkmkarlsruhe/NextcloudVideo_Converter) | Nextcloud video converter (2021). |
| [nextcloud-printer](https://github.com/zkmkarlsruhe/nextcloud-printer) | Nextcloud printing app (2019). |
| [mapping-open-source](https://github.com/zkmkarlsruhe/mapping-open-source) | Research: Open source in museums. |

---

## Templates

This repository includes templates for consistent documentation across ZKM projects.

### Using the Templates

**For new repositories:**
```bash
# Copy README template
cp templates/README.md your-repo/README.md

# Copy license (choose one)
cp templates/LICENSE-MIT your-repo/LICENSE
# or
cp templates/LICENSE-BSD your-repo/LICENSE

# Copy contribution guidelines
cp templates/CONTRIBUTING.md your-repo/CONTRIBUTING.md
```

**For the "Funded by" section (place at bottom of README):**
```html
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

### Available Templates

| File | Purpose |
|------|---------|
| [templates/README.md](templates/README.md) | Standard README for repos |
| [templates/README-deprecated.md](templates/README-deprecated.md) | Notice for repos moved to GitHub |
| [templates/CONTRIBUTING.md](templates/CONTRIBUTING.md) | Contribution guidelines |
| [templates/LICENSE-MIT](templates/LICENSE-MIT) | MIT License |
| [templates/LICENSE-BSD](templates/LICENSE-BSD) | BSD Simplified License |
| [templates/.github/ISSUE_TEMPLATE/](templates/.github/ISSUE_TEMPLATE/) | Issue templates |

### Badges

```markdown
<!-- ZKM Badge -->
[![ZKM](https://img.shields.io/badge/ZKM-Karlsruhe-blue)](https://zkm.de)

<!-- License Badges -->
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![License: BSD](https://img.shields.io/badge/License-BSD-blue.svg)](LICENSE)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE)
```

See [docs/badges.md](docs/badges.md) for complete badge reference including logo variants.

### Standard Copyright

```
Copyright (c) 2026 ZKM | Karlsruhe
```

---

## License Strategy

| Project Type | License |
|-------------|---------|
| Default / New Projects | MIT |
| openFrameworks Addons | BSD Simplified |
| Standalone Applications | GPL-3.0 |
| Hardware Designs | CC BY-SA 4.0 |

---

## Contact

- **Website:** [zkm.de](https://zkm.de)
- **Wikipedia:** [ZKM Center for Art and Media Karlsruhe](https://en.wikipedia.org/wiki/ZKM_Center_for_Art_and_Media_Karlsruhe)
- **Instagram:** [@zkmkarlsruhe](https://www.instagram.com/zkmkarlsruhe/)
- **YouTube:** [ZKMkarlsruhe](https://www.youtube.com/user/ZKMkarlsruhe)
- **LinkedIn:** [ZKM](https://www.linkedin.com/company/zkm-zentrum-f%C3%BCr-kunst-und-medien)
- **Facebook:** [zkmkarlsruhe](https://www.facebook.com/zkmkarlsruhe)
