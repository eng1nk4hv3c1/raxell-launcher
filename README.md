# RAXEL LAUNCHER

<div align="center">

  <img width="180" height="180" alt="RAXEL Launcher Logo" src="https://github.com/user-attachments/assets/cb81fbcd-45a5-45e8-bf31-33d87697ba34" />

  <h1 align="center">RAXEL LAUNCHER</h1>

  <p align="center">
    <strong>One Library. Every Achievement. Your Cloud.</strong>
  </p>

  <p align="center">
    Your games. Your achievements. Your saves. All in one place.
  </p>

  <p align="center">
    <a href="https://github.com/eng1nk4hv3c1/raxell-launcher">GitHub Repository</a>
    ·
    <a href="#features">Features</a>
    ·
    <a href="#roadmap">Roadmap</a>
    ·
    <a href="#building-from-source">Build from Source</a>
  </p>

  ![License](https://img.shields.io/github/license/eng1nk4hv3c1/raxell-launcher?style=flat-square)
  ![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux-red?style=flat-square)
  ![Status](https://img.shields.io/badge/status-in%20development-orange?style=flat-square)
  ![Open Source](https://img.shields.io/badge/open%20source-yes-red?style=flat-square)

</div>

---

## About RAXEL

**RAXEL Launcher** is an open-source gaming platform designed to bring your entire gaming experience into one place.

Manage your PC games, discover your library, track achievements, organize your saves, and keep your gaming progress synchronized across devices.

Built on the existing Hydra Launcher technology stack, RAXEL aims to preserve proven functionality while introducing its own identity, architecture improvements, and cloud ecosystem.

RAXEL is developed using:

- **Electron** for the desktop application.
- **React** for the user interface.
- **TypeScript** for application logic.
- **Rust** for native functionality and performance.
- **SQLite** for local data management.
- **libtorrent** for the existing torrent engine.

RAXEL follows an offline-first philosophy: your library and local data remain accessible even when you are disconnected from the internet.

## Features

> RAXEL is actively under development. The features below describe the existing upstream functionality being retained, the planned RAXEL functionality, and the direction of the project. Not every feature is currently available in RAXEL.

### 🎮 Game Library

A unified place for your games.

- Add custom games and executable files.
- Organize games with collections and favorites.
- Import Steam libraries, playtime, and achievements.
- Connect Epic Games accounts.
- Scan drives for installed games.
- Track playtime.
- Customize game covers, backgrounds, logos, and icons.
- Create desktop and Steam shortcuts.

### 🏆 Achievements

Your gaming achievements, together in one place.

- Centralized achievement tracking.
- Steam and Epic Games achievement integration.
- In-game achievement notifications.
- Custom achievement unlock sounds.
- RetroAchievements support.
- RPCS3 and shadPS4 trophy tracking.
- Achievement history and statistics.

RAXEL aims to preserve and extend the existing achievement infrastructure rather than unnecessarily rebuilding it from scratch.

### ☁️ RAXEL Cloud

**Your cloud. Your storage. Your control.**

RAXEL Cloud is designed around a simple principle: users should be able to use their own cloud storage accounts instead of depending on a subscription-based storage service operated by RAXEL.

Planned integrations:

- Google Drive
- MEGA
- Microsoft OneDrive
- Dropbox
- WebDAV
- SFTP

Planned capabilities:

- Automatic game save backups.
- Cross-device save synchronization.
- Manual backup and restore.
- Multiple cloud providers.
- Primary and secondary storage configuration.
- Backup version history.
- File integrity verification.
- Conflict detection and resolution.
- Emulator save and memory card backups.

**No mandatory RAXEL storage subscription. No required RAXEL-hosted save storage.**

Your cloud accounts remain yours.

### 💾 Save Management

Protect your gaming progress.

- Automatic save discovery.
- Game save backup and restore.
- Manual save directory configuration.
- Scheduled backups.
- Save version history.
- Cloud synchronization.
- Conflict resolution.
- File integrity verification.

Existing save management components, including compatible Ludusavi functionality, will be reused wherever practical.

### 🕹️ Classic Games & Emulation

Bring your classic games into the same library.

The project aims to retain and extend existing emulator integrations, including:

- DuckStation
- PCSX2
- RPCS3
- shadPS4
- PPSSPP
- Dolphin
- RetroArch

Planned functionality includes ROM library scanning, metadata matching, artwork, emulator management, and unified game launching.

### 📊 Statistics

Understand your gaming activity.

Planned statistics include:

- Total games.
- Total playtime.
- Achievement progress.
- Recently played games.
- Most played games.
- Gaming activity history.

### 🎨 Personalization

Make RAXEL yours.

- Dark-themed interface.
- Customizable appearance.
- Modern red-accented visual identity.
- Interface localization.
- Custom game artwork.
- Configurable notifications.

---

## Roadmap

RAXEL is being developed incrementally, with an emphasis on reliability and preserving existing functionality.

| Phase | Development goal | Status |
|---|---|---|
| 1 | Repository audit and architecture analysis | Planned |
| 2 | RAXEL branding and application identity | In progress |
| 3 | Preserve existing game library and integrations | In progress |
| 4 | Achievement system integration | Planned |
| 5 | Cloud provider architecture | Planned |
| 6 | Cloud Save backup and restore | Planned |
| 7 | Multi-provider synchronization | Planned |
| 8 | Cloud achievement backup | Planned |
| 9 | UI/UX improvements | Planned |
| 10 | Security, performance and testing | Planned |

Roadmap statuses will be updated as features are implemented and verified.

## Technology Stack

| Technology | Purpose |
|---|---|
| Electron | Desktop application |
| React | User interface |
| TypeScript | Application development |
| Rust | Native functionality |
| SQLite | Local database |
| libtorrent | Torrent engine |
| Ludusavi | Game save management integration |

## Privacy & Security

Your data belongs to you.

RAXEL is designed with privacy and local data ownership in mind.

Our development priorities include:

- Local-first data management.
- Secure credential storage.
- OAuth-based authentication where supported.
- No hardcoded API secrets.
- No unnecessary collection of personal information.
- Secure cloud synchronization.
- File integrity verification.
- Safe backup and restore operations.

Cloud provider credentials should be stored using appropriate operating system security facilities rather than plaintext configuration files.

## Building from Source

RAXEL is built on the Electron, React, TypeScript, and Rust ecosystem.

### Requirements

- Node.js
- Yarn
- Rust toolchain
- Git
- C++ build tools

**Windows:**
- Visual Studio C++ Build Tools.

**Linux:**
- GCC or Clang.
- Required system development libraries.

### Installation

Clone the repository:

```bash
git clone https://github.com/eng1nk4hv3c1/raxell-launcher.git

cd raxell-launcher
```

Install dependencies:

```bash
yarn install
```

Start development mode:

```bash
yarn dev
```

### Build

Run the project build:

```bash
yarn build
```

Windows build:

```bash
yarn build:win
```

Linux build:

```bash
yarn build:linux
```

Available scripts and platform-specific requirements may change as development progresses. Refer to `package.json` for the current commands.

## Project Origins & Attribution

RAXEL is an independent project derived from the open-source Hydra Launcher codebase.

The project retains and builds upon existing upstream technologies and components where appropriate.

We respect the original authors, contributors, licenses, and attribution requirements.

RAXEL is not an official Hydra Launcher product and is not affiliated with the original Hydra Launcher project.

Original project:

https://github.com/hydralauncher/hydra

## Contributing

Contributions, bug reports, ideas, and suggestions are welcome.

If you want to contribute:

1. Fork the repository.
2. Create a feature branch.
3. Make your changes.
4. Test your changes.
5. Submit a pull request.

Please keep changes focused, document important architectural decisions, and avoid introducing unnecessary dependencies.

## License

RAXEL uses the MIT License, subject to the actual license files and applicable upstream licensing obligations.

See the [LICENSE](LICENSE) file for details.

---

<div align="center">

  **RAXEL LAUNCHER**

  *One Library. Every Achievement. Your Cloud.*

  Built for gamers. Designed for freedom.

</div>
