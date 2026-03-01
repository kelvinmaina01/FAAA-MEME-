# How Faaaaaahhh Works

I've analyzed the source code and here is a breakdown of how the Faaaaaahhh extension works before you launch it:

## 1. The Core Architecture
The extension is built on an **event-driven architecture**. It uses **Watchers** that "listen" to specific events inside VS Code and send triggers to a central **Sound Player**.

## 2. How it Detects Errors (Watchers)
- **Diagnostic Watcher**: This is the heart of the extension. It monitors your code as you type.
    - **Syntax vs. Semantic**: It can tell the difference between a simple typo (Syntax Error) and a complex logic error (Semantic Error). Typos trigger a "gentle" sound, while real logic errors trigger the full FAAAH.
    - **The Diff Engine**: It only plays a sound when the error count **increases**. If you have 5 errors and fix one, it stays silent. If you go from 5 to 6, it screams.
- **Terminal Watcher**: Listens for failed commands. If you type a command that doesn't exist or a script fails (non-zero exit code), it triggers a sound.
- **Task & Debug Watchers**: If a build task fails or a debug session crashes, the extension catches it and plays a sound.

## 3. The Sound Logic (Tier System)
The extension doesn't just play one sound. It has an intensity scale:
- **Tier 1 (1 error)**: A soft, low-intensity sound.
- **Tier 2 (2–4 errors)**: A mid-range sound.
- **Tier 3 (5+ errors)**: The full high-frequency FAAAH chaos.

## 4. Smart Features
- **Sound Packs**: You have three built-in modes: Meme (Classic), Rage (Aggressive), and Chill (Softer tones).
- **Quiet Hours**: You can set a time range (e.g., 9:00 AM to 5:00 PM) where the extension remains silent automatically.
- **Cooldown**: Prevents the extension from "spamming" sounds if many errors happen at once.
- **Victory Mode**: An optional feature that plays a satisfying sound when you finally clear all errors in a file.

## 5. Cross-Platform
The Sound Player is designed to work natively on **Windows** (via PowerShell), **macOS** (via `afplay`), and **Linux** (via `paplay`), ensuring it sounds great no matter the OS.

Everything is configured through a premium-looking Settings Panel or directly via VS Code's `settings.json`. You're all set for a successful launch!
