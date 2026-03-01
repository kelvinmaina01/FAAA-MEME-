<p align="center">
  <img src="https://iili.io/qqE5H1S.md.png" alt="FAAAAHHH Meme Sound Extension" width="100%"/>
</p>

<p align="center">
  <a href="https://marketplace.visualstudio.com/items?itemName=kelvinmaina01.faaaaaahhh">
    <img src="https://img.shields.io/visual-studio-marketplace/v/kelvinmaina01.faaaaaahhh?style=for-the-badge&color=FF3B3B&label=Marketplace" alt="Marketplace"/>
  </a>
  <a href="https://marketplace.visualstudio.com/items?itemName=kelvinmaina01.faaaaaahhh">
    <img src="https://img.shields.io/visual-studio-marketplace/i/kelvinmaina01.faaaaaahhh?style=for-the-badge&color=2A2E3A&label=Installs" alt="Installs"/>
  </a>
  <a href="https://github.com/kelvinmaina01/FAAA-MEME-">
    <img src="https://img.shields.io/github/stars/kelvinmaina01/FAAA-MEME-?style=for-the-badge&color=FFDD00" alt="GitHub stars"/>
  </a>
  <a href="https://ko-fi.com/kelvinmaina01">
    <img src="https://img.shields.io/badge/Support_this_repository-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black" alt="Support this repository"/>
  </a>
</p>

<p align="center">
  <a href="https://github.com/kelvinmaina01/FAAA-MEME-/stargazers">
    <img src="https://img.shields.io/github/stars/kelvinmaina01/FAAA-MEME-?style=for-the-badge&color=FF6B6B" alt="GitHub stars"/>
  </a>
</p>

---

## 🎵 Auditory Feedback for Diagnostic Chaos

**Faaaaaahhh** is a Visual Studio Code extension that turns developer suffering into high-fidelity entertainment. Every time an error appears in your editor, it plays the iconic **FAAAH** meme sound. Warnings get a gentler, slightly less judgmental **AA**.

### ✨ Key Features

- **🎯 Severity Tiers** - Syntax errors get gentle feedback, while error avalanches trigger chaos
- **🎵 Smart Audio Engine** - Native Windows, macOS, and Linux support with realistic overlapping sounds
- **⚙️ Settings Panel** - Graphical UI for volume, cooldowns, quiet hours, and sound packs
- **🎧 Sound Packs** - Switch between Meme, Rage, and Chill sound packs
- **🎮 Terminal Watcher** - Terminal command failures trigger sounds too
- **🏆 Victory Mode** - Celebratory sound when you finally fix all errors in a file

---

## 🚀 How It Works

The extension monitors four VS Code event channels:

| Channel | Trigger | Sound |
|---------|---------|-------|
| **Diagnostics** | New errors/warnings appear | FAAAH (errors) / AA (warnings) |
| **Tasks** | Build task fails (non-zero exit) | FAAAH |
| **Terminal** | Command not found or script fails | AHHHH |
| **Debug** | Debug session crashes | FAAAH |

**The Diff Engine:** Only triggers sounds when error counts *increase* in a file.

---

## 🎛️ Configuration

### Quick Settings (via Settings Panel)
- **Master Toggle**: Enable/disable all sounds
- **Volume Control**: 0-100% global volume
- **Quiet Hours**: Auto-mute during specific hours
- **Cooldown Timer**: Minimum time between sounds
- **Sound Packs**: Switch between Meme, Rage, or Chill packs
- **Tier System**: Different sounds for 1 error vs 5+ errors

### settings.json
```json
{
  "faaaaahhh.enabled": true,
  "faaaaahhh.volume": 80,
  "faaaaahhh.soundPack": "meme",
  "faaaaahhh.quietHoursStart": "22:00",
  "faaaaahhh.quietHoursEnd": "08:00",
  "faaaaahhh.victoryEnabled": false
}
```

---

## 🚀 Installation

**Marketplace:** Search for `Faaaaaahhh` in VS Code Extensions

**Manual:**
```bash
code --install-extension faaaaaahhh-0.3.7.vsix
```

---

<p align="center">
  <img src="https://raw.githubusercontent.com/kelvinmaina01/FAAA-MEME-/main/assets/icon.png" width="64" height="64"/><br/>
  <sub>Built with ❤️ by <a href="https://github.com/kelvinmaina01">kelvinmaina01</a></sub><br/>
  <a href="LICENSE">MIT License</a>
</p>

<p align="center">
  <sub>If this extension makes your coding less painful, consider:</sub>
  <br>
  <a href="https://ko-fi.com/kelvinmaina01">
    <img src="https://img.shields.io/badge/Support_this_repository-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black" alt="Support this repository"/>
  </a>
  <br>
  <a href="https://github.com/kelvinmaina01/FAAA-MEME-">
    <img src="https://img.shields.io/badge/Star_this_repo-FFD166?style=for-the-badge&logo=github&logoColor=white" alt="Star this repository"/>
  </a>
</p>


