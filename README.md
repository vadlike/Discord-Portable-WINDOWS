# 🚀 Discord Portable 1.0.9228 + Vencord ![visitors](https://visitor-badge.laobi.icu/badge?page_id=vadlike.Discord-Portable-WINDOWS)

Portable Discord build with local data storage and Vencord integration.

## ✨ Highlights
- ✅ Fully portable launcher (`DiscordPortable.cmd`)
- ✅ Local data storage inside `Data\` (portable-friendly)
- ✅ Auto-detects newest `app-*` folder on launch
- ✅ Vencord already integrated
- ✅ One-click Vencord repatch after Discord updates (`vencordrepatch.bat`)
- ✅ `VencordInstallerCli.exe` included next to launcher
- ✅ No `app-*` symlink tricks used

## 📦 Included Files
- `DiscordPortable.cmd` — main launcher
- `vencordrepatch.bat` — repatch Vencord after updates
- `VencordInstallerCli.exe` — Vencord installer CLI
- `Update.exe`, `RELEASES`, `installer.db`
- `app-1.0.9219\...` (Discord app folder; newer `app-*` appears after update)

## 🧠 How It Works
- Launcher redirects runtime paths to local `Data\` folders.
- `%APPDATA%\discord` is redirected to:
  `Data\AppData\Roaming\discord`
- On update, Discord creates a new `app-*` folder.
- `DiscordPortable.cmd` always picks the newest available `app-*`.

## 🛠️ Quick Start
1. Extract the archive anywhere.
2. Run `DiscordPortable.cmd`.
3. Log in and use Discord normally.

## 🔁 After Discord Updates
1. Let Discord finish updating.
2. Run `vencordrepatch.bat`.
3. Start Discord again.

## 📁 Data Locations
- `Data\AppData\Roaming\discord`
- `Data\AppData\Local`
- `Data\Temp`
- `Data\VencordData`

## ⚠️ Notes
- On first launch, if `%APPDATA%\discord` already exists as a normal folder, it is backed up once.
- SmartScreen may show a warning on some systems.
- Built for Windows portable usage.

## ❤️ Credits
- Author tag in launcher: **VADLIKE**
- Vencord project: https://github.com/Vendicated/Vencord

