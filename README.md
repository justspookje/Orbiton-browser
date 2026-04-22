# 🌐 Orbitom Browser

A Chromium-based browser built with Electron.

## Features
- Multi-tab browsing with tab management
- Custom address bar with search (Google fallback)
- Back / Forward / Reload / Home navigation
- New Tab page with shortcuts
- Custom frameless window with traffic-light controls
- Loading progress bar
- Status bar with HTTPS indicator

## Build the .exe (Windows)

### Requirements
- [Node.js](https://nodejs.org) v18 or newer
- Windows 10/11 x64

### Steps
1. Extract this folder somewhere on your PC
2. Double-click **BUILD.bat**
3. Wait for it to finish (first run downloads Electron — ~200MB)
4. Find the installer at: `dist\Casperuim Setup 1.0.0.exe`

### Or manually via PowerShell / CMD:
```
npm install
npm run build
```

### Just want to run it without building?
```
npm install
npm start
```

## Project structure
```
casperuim/
├── main.js          ← Electron main process
├── preload.js       ← IPC bridge
├── renderer/
│   └── index.html   ← Browser UI
├── assets/
│   └── icon.ico     ← App icon
├── package.json
└── BUILD.bat        ← One-click builder
```
