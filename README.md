<div align="center">

# Min Browser

<p align="center">
  <b>A fast, minimal browser that protects your privacy.</b>
</p>

[![Build Status](https://github.com/minbrowser/min/actions/workflows/build-packages.yml/badge.svg)](https://github.com/minbrowser/min/actions/workflows/build-packages.yml)
[![Latest Release](https://img.shields.io/github/v/release/minbrowser/min?include_prereleases&style=flat&color=blue)](https://github.com/minbrowser/min/releases)
[![Downloads][DownloadsBadge]][DownloadsUrl]
[![Node Version](https://img.shields.io/badge/node-%3E%3D20.0.0-brightgreen.svg)](https://nodejs.org/)
[![License](https://img.shields.io/badge/license-Apache--2.0-blue.svg)](LICENSE.txt)
[![Discord][DiscordBadge]][DiscordUrl]

</div>

---

Min is a fast, lightweight browser designed to minimize distractions and protect your privacy. Built on Electron, Min features an uncluttered interface and powerful built-in tools.

## Key Features

- 🔍 **Full-text search**: Search through the content of pages you've visited.
- 🛡️ **Ad and tracker blocking**: Block ads, trackers, and third-party scripts automatically.
- 📖 **Automatic reader view**: Read articles without distractions, sidebars, or ads.
- 📑 **Tasks (tab groups)**: Organize tabs into task groups for focused workflows.
- 🏷️ **Bookmark tagging**: Easily tag and search your saved bookmarks.
- 🔐 **Password manager integration**: Works with 1Password, Bitwarden, and built-in password storage.
- 🌙 **Dark theme**: Automatically matches your system appearance or manual dark mode preferences.

---

## Screenshots

<div align="center">

<img alt="The search bar, showing information from DuckDuckGo" src="http://minbrowser.org/tour/img/searchbar_duckduckgo_answers.png" width="650"/>

<br/><br/>

<img alt="The Tasks Overlay" src="http://minbrowser.org/tour/img/tasks.png" width="650"/>

<br/><br/>

<img alt="Reader View" src="https://user-images.githubusercontent.com/10314059/53312382-67ca7d80-387a-11e9-9ccc-88ac592c9b1c.png" width="650"/>

</div>

---

## Installing

You can download official prebuilt binaries for Linux, macOS, and Windows on the **[Releases Page](https://github.com/minbrowser/min/releases)**, or visit the [official website](https://minbrowser.org/).

### Platform Instructions

- **Linux (Debian/Ubuntu)**: `sudo dpkg -i /path/to/min_*.deb`
- **Linux (RedHat/Fedora)**: `sudo rpm -i /path/to/min_*.rpm --ignoreos`
- **Arch Linux**: Install via [AUR](https://aur.archlinux.org/packages/min-browser-bin).
- **Raspberry Pi / ARM**: Available via [Pi-Apps](https://github.com/Botspot/pi-apps) or directly from [Releases](https://github.com/minbrowser/min/releases).
- **macOS**: Download `.dmg` or `.zip`, move to `/Applications`.
- **Windows**: Download setup `.exe` or portable `.zip`.

---

## Quick Start for Developers

To run Min locally from source code:

1. **Prerequisites**: Ensure [Node.js](https://nodejs.org) (v20 or higher) and `npm` are installed.
2. **Clone repository**:
   ```bash
   git clone https://github.com/minbrowser/min.git
   cd min
   ```
3. **Install dependencies**:
   ```bash
   npm install
   ```
4. **Start application**:
   ```bash
   npm run start
   ```

> **Tip:** While running in development mode, press `Ctrl+Alt+R` (`Cmd+Opt+R` on macOS) to reload the UI.

---

## Building Binaries (Cross-Device)

Min includes scripts to build native packages for multiple operating systems and CPU architectures:

| Platform / Architecture | Target Package | Build Command |
| :--- | :--- | :--- |
| **Windows (x64)** | Setup Installer (`.exe`) / Zip (`.zip`) | `npm run buildWindows` |
| **macOS (Intel x86_64)** | Portable Zip (`.zip`) | `npm run buildMacIntel` |
| **macOS (Apple Silicon Arm64)** | Portable Zip (`.zip`) | `npm run buildMacArm` |
| **Linux (Debian / Ubuntu amd64)** | Debian Package (`.deb`) | `npm run buildDebian` |
| **Linux (RedHat / Fedora x86_64)** | RPM Package (`.rpm`) | `npm run buildRedhat` |
| **Linux (Universal AppImage)** | AppImage (`.AppImage`) | `npm run buildAppImage` |
| **Linux (ARM64 / Raspberry Pi 64-bit)** | Debian Package (`.deb`) | `npm run buildLinuxArm64` |
| **Linux (Raspberry Pi 32-bit)** | Debian Package (`.deb`) | `npm run buildRaspi` |
| **Build All Packages** | All supported targets | `npm run buildAll` |

### System Prerequisites for Building

- **macOS**: Requires Xcode and Command Line Tools. Set SDK root if needed:
  ```bash
  export SDKROOT=$(xcrun --sdk macosx --show-sdk-path)
  ```
- **Windows**: Requires Visual Studio with C++ Build Tools installed.

---

## Getting Started & Resources

* **[Wiki Documentation](https://github.com/minbrowser/min/wiki)**: Feature guide, keyboard shortcuts, and [FAQ](https://github.com/minbrowser/min/wiki/FAQ).
* **[Userscripts Guide](https://github.com/minbrowser/min/wiki/userscripts)**: Extend Min with custom userscripts.
* **[Community Discord](https://discord.gg/bRpqjJ4)**: Join for support, discussions, and dev updates.

---

## Contributing

We welcome contributions of all kinds!

- **Report Bugs & Feedback**: Open an issue on [GitHub Issues](https://github.com/minbrowser/min/issues/new/choose).
- **Architecture Overview**: Learn about Min's design in the [Wiki Architecture guide](https://github.com/minbrowser/min/wiki/Architecture).
- **Code Style**: Min follows [Standard JS](https://github.com/standard/standard). Run `npm test` to lint your code before opening a pull request.
- **Translations**: Translate Min into your language by adding or updating files in `localization/languages/`.

---

## Sponsors

Min is made possible by these sponsors:

| [<img src="https://avatars.githubusercontent.com/u/6592155?v=4" width="40">](https://github.com/blackgwe) | [<img src="https://avatars.githubusercontent.com/u/49724477?v=4" width="40">](https://github.com/rafel-ioli) | [<img src="https://avatars.githubusercontent.com/u/237596?v=4" width="40">](https://github.com/idoru) |
| :--- | :--- | :--- |
| [@blackgwe](https://github.com/blackgwe) | [@rafel-ioli](https://github.com/rafel-ioli) | [@idoru](https://github.com/idoru) |

[Become a sponsor](https://github.com/sponsors/PalmerAL)

---

## License

Min is open source software licensed under the [Apache-2.0 License](LICENSE.txt).

[DiscordBadge]: https://img.shields.io/discord/764269005195968512.svg?label=Discord&logo=discord&logoColor=white
[DiscordUrl]: https://discord.gg/bRpqjJ4
[DownloadsBadge]: https://img.shields.io/github/downloads/minbrowser/min/total.svg
[DownloadsUrl]: https://github.com/minbrowser/min/releases
