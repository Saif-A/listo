**Listo**

Listo is an ultra-fast, Windows launcher for apps, files, folders, windows settings and even custom commands. Use `Ctrl + Space` to activate the launcher, type what you need to find and Listo will find it instantly. Listo can be used to search important file types only (the default mode) , or you can search all file types if you enable the "Include all file types" option in Listo settings.

**Quick Start**
1. Open [the latest release page](https://github.com/Saif-A/listo/releases/latest) and download `Listo_Setup_1.0.43.exe`.
2. Launch Listo from the Start Menu if it doesn't start automatically.
3. press `Ctrl + Space` to show the launcher.
4. Type part of a file or folder name to find it, then press `Enter` to open it or `Shift + Enter` to open its containing folder.
5. if you like, you can activate a quick filter before you search by:

    - pressing `Space` to enter folder search mode
    - typing `c` then `Space` to search drive C: only (works for any local drive)
    - typing `cf` then `Space` to search drive C: for folders only (works for any local drive)
    - typing `.pdf` then `Space` to filter PDF files (works for any file extension)
    - typing `ss` then `Space` to search for shortcuts and apps
    - use it as a calculator by typing a math expression such as `2+2` or `sqrt(16)` and pressing `Enter` to copy the result to the clipboard
    - typing `/` to open the command palette, or typing a command keyword directly to run a custom command (if configured in settings)
    - when a Save/Open dialog is focused, activating Listo will automatically switch to folder-search mode to help you navigate to the right location quickly.

**Features**
1. Instant activation with double-tap `Ctrl` or `Ctrl + Space`
2. Fast fuzzy search with typo-tolerant, multi-word matching
3. Smart ranking based on rules, file types, paths, extensions, and recent use
4. Background indexing of fixed drives with exclusions and live updates via `ReadDirectoryChangesW`
5. Folder search plus configurable file-type indexing, including optional `Include all file types`
6. Keyboard-first launching, containing-folder open, and Windows shell context menu access
7. Built-in calculator and custom commands in keyword or slash mode
8. Dedicated folder navigation mode for Save/Open dialogs
9. Tray menu, themes, settings pages, and Index Statistics tools
10. Startup initialization prompt until the first index is ready
11. Built-in update checks with release notes, checksum verification, silent installer handoff, and relaunch

**Notes**
- This repository is the public distribution endpoint for binaries, release notes, and update metadata.
- The Listo source code is not hosted in this repository.
- In-app updates read [latest.json](https://raw.githubusercontent.com/Saif-A/listo/main/latest.json) to discover the current stable installer.

**Links**
- Latest release: [https://github.com/Saif-A/listo/releases/latest](https://github.com/Saif-A/listo/releases/latest)
- Public repo: [https://github.com/Saif-A/listo](https://github.com/Saif-A/listo)
- All releases: [https://github.com/Saif-A/listo/releases](https://github.com/Saif-A/listo/releases)
- Latest manifest: [latest.json](https://raw.githubusercontent.com/Saif-A/listo/main/latest.json)

Attribution: Saif A.
