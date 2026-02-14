# InstantScreensharePlus

Instantly screenshare when joining a voice channel with support for desktop sources, windows, and video input devices (cameras, capture cards).

## Features

- Auto-start screenshare when joining voice channels
- Auto-enable camera when joining voice channels
- Auto-mute/unmute when joining/leaving voice channels
- Auto-toggle push-to-talk mode
- Supports desktop sources, windows, and video input devices
- Toolbox actions for quick toggling







## Installation 

### 🪄 Installation Wizard
The easiest way to install this plugin is to use the **[Plugin Installer Generator](https://bluscream-vencord-plugins.github.io)**. 
Simply select this plugin from the list and download your custom install script.

### 💻 Manual Installation (PowerShell)
Alternatively, you can run this snippet in your Equicord/Vencord source directory:
```powershell
$ErrorActionPreference = "Stop"
winget install -e --id Git.Git
winget install -e --id OpenJS.NodeJS
npm install -g pnpm
git clone https://github.com/Equicord/Equicord Equicord
New-Item -ItemType Directory -Force -Path "Equicord\src\userplugins" | Out-Null
git clone https://github.com/bluscream-vencord-plugins/blu-instantScreenshare.git -b "main" "Equicord\src\userplugins\blu-instantScreenshare"
cd "Equicord"
npm install -g pnpm
pnpm install --frozen-lockfile
pnpm build
pnpm buildWeb
pnpm inject
```
