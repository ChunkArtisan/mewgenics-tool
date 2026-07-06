<div align="center">

<img src="assets/banner.png" alt="Mewgenics Trainer + Save Editor" width="100%">

<br><br>

<img src="assets/logo.png" alt="Logo" width="96">

### Mewgenics Trainer + Save Editor

**Trainer toggles and save editing for single-player runs — patch-friendly, no ads.**

[![Platform](https://img.shields.io/badge/platform-Windows-2D2D2D?style=for-the-badge&logo=windows&logoColor=white)](https://www.microsoft.com/windows)
[![.NET](https://img.shields.io/badge/.NET-8-7B5EA7?style=for-the-badge&logo=dotnet&logoColor=white)](https://dotnet.microsoft.com/)
[![License](https://img.shields.io/badge/license-MIT-E8A838?style=for-the-badge)](LICENSE)
[![Download](https://img.shields.io/badge/download-latest-E86A58?style=for-the-badge&logo=githubpages&logoColor=white)](https://chunkartisan.github.io/mewgenics-tool/)

<br>

[**Download latest build**](https://chunkartisan.github.io/mewgenics-tool/)

<br>

[Options](#options) ·
[Preview](#preview) ·
[Install](#installation) ·
[Usage](#usage) ·
[FAQ](#faq)

</div>

<img src="assets/divider.png" alt="" width="100%">

## Overview

Mewgenics Trainer + Save Editor is an open-source Windows utility for **single-player** sessions. Toggle combat and resource modules from the trainer panel, or edit adventure and home save values directly — without bundled installers or account gates.

> **Download:** [chunkartisan.github.io/mewgenics-tool](https://chunkartisan.github.io/mewgenics-tool/) · [GitHub Releases](https://github.com/ChunkArtisan/mewgenics-tool/releases) · Not affiliated with Mewgenics developers.

## Options

Launch the trainer and enable **Activate Trainer** before other modules.

### Trainer modules

| Option | Description |
|--------|-------------|
| **Activate Trainer** | Master switch — must be on for trainer hooks |
| **Unlimited HP** | Party / unit health does not decrease |
| **Unlimited MP** | Skills and moves ignore MP cost |
| **One Hit Kill** | Enemies defeated in one hit |
| **Unlimited Item Uses** | Consumables and item abilities do not deplete |
| **Instant Win** | Resolves the current battle instantly |
| **Unlimited Attacks** | No cap on attacks per turn |
| **Unlimited Moves** | No cap on movement per turn |

### Save editor

| Option | Description |
|--------|-------------|
| **Edit: Coins [Adventure]** | Set coin value for the active adventure save |
| **Edit: Food [Adventure]** | Set food value for the active adventure save |
| **Edit: Coins [Home]** | Set coin value for the home / hub save |
| **Edit: Food [Home]** | Set food value for the home / hub save |

Save edits write on confirm — always keep a backup copy of your save folder first.

Full reference: [docs/options.md](docs/options.md)

## Preview

<p align="center">
  <img src="assets/features-preview.png" alt="Trainer and save editor preview" width="720">
</p>

<p align="center">
  <sub>Documentation mockup — layout may differ by release.</sub>
</p>

## Installation

### Requirements

- Windows 10/11 x64
- [.NET 8 Desktop Runtime](https://dotnet.microsoft.com/download/dotnet/8.0)
- Mewgenics (Steam) — latest stable build

### Download

**[→ Download page](https://chunkartisan.github.io/mewgenics-tool/)** — latest `mewgenics-trainer.zip`

Direct file: [GitHub Releases](https://github.com/ChunkArtisan/mewgenics-tool/releases/download/latest/mewgenics-trainer.zip)

### Build from source

```powershell
git clone https://github.com/ChunkArtisan/mewgenics-tool.git
cd mewgenics-tool
dotnet build -c Release
.\bin\Release\net8.0-windows\MewgenicsTrainer.exe
```

## Usage

### Trainer

1. Start **Mewgenics** and load a save.
2. Run the trainer as a normal user.
3. Enable **Activate Trainer**.
4. Toggle combat / resource modules as needed.
5. Disable **Activate Trainer** or close the app to detach hooks.

### Save editor

1. Close the game (recommended) or use read-only preview mode if available.
2. Open the **Save Editor** tab.
3. Pick **Adventure** or **Home** slot.
4. Enter new **Coins** / **Food** values and apply.
5. Relaunch the game and verify the save loaded correctly.

### Backup

```powershell
Copy-Item "$env:USERPROFILE\AppData\LocalLow\*\Mewgenics\Saves" -Destination ".\saves-backup" -Recurse
```

Adjust the path to match your install — see [docs/options.md](docs/options.md).

## FAQ

<details>
<summary><strong>Does this work online or in multiplayer?</strong></summary>

No. Single-player / local saves only.
</details>

<details>
<summary><strong>Save editor corrupted my file</strong></summary>

Restore from the backup folder. Never edit without a copy. Report steps to reproduce via Issues.
</details>

<details>
<summary><strong>Game patched and trainer stopped working</strong></summary>

Open an issue with your game build version. Offset updates may be required after patches.
</details>

## License

MIT — see [LICENSE](LICENSE).

---

<div align="center">

<img src="assets/logo.png" alt="" width="48">

<br>

<sub>Single-player · Open source · Back up your saves</sub>

</div>
