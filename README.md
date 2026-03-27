# Listo

Listo is a fast, keyboard-first Windows launcher for files, folders, commands, and built-in Windows surfaces.

By Saif A.

## Quick Start

### Install

1. Download [Listo_Setup_1.0.36.exe](https://github.com/Saif-A/listo/releases/download/v1.0.36/Listo_Setup_1.0.36.exe).
2. Run the installer.
3. Launch Listo from the Start Menu.

### Activate

- Press `Ctrl` twice quickly
- Or press `Ctrl` + `Space`
- Press the same shortcut again to hide Listo
- On first launch, if Listo says it is initializing the index, wait a few seconds until search becomes available
- Press `Escape` to clear the current query first; press it again on an empty box to hide Listo

### Keyboard Shortcuts

- `Ctrl` + `Ctrl` or `Ctrl` + `Space`: show or hide Listo
- `Ctrl` + `A`: select all text in the search box
- `Up` / `Down`: move through results
- `Enter`: open the selected result
- `Shift` + `Enter`: open the selected result's containing folder
- `Backspace` on empty input: clear an active filter or exit a temporary mode
- `Escape`: clear the current query first; if it is already empty, hide the launcher

## Download

- Latest installer: [Listo_Setup_1.0.36.exe](https://github.com/Saif-A/listo/releases/download/v1.0.36/Listo_Setup_1.0.36.exe)
- All public releases: [GitHub Releases](https://github.com/Saif-A/listo/releases)
- Update manifest used by the app: [latest.json](https://raw.githubusercontent.com/Saif-A/listo/main/latest.json)

## Install And Update

1. Download `Listo_Setup_1.0.36.exe`.
2. Run the installer.
3. Launch Listo from the Start Menu.
4. Use `Ctrl` + `Ctrl` or `Ctrl` + `Space` to show or hide the launcher.
5. Future versions can be installed over the top, or accepted from Listo's built-in updater.

## What Listo Does

Listo is designed for quick everyday Windows navigation without reaching for the mouse. It can:

- find files and folders quickly with fuzzy matching
- launch results directly or open their containing folders
- filter searches by drive, folder-only mode, shortcuts, or extension
- run custom commands from keywords or a slash command palette
- evaluate math expressions inline
- jump folders inside Save and Open dialogs
- stay available from the system tray
- keep its file index fresh in the background
- check for app updates automatically

## Features

- Instant activation with double-tap `Ctrl` or `Ctrl` + `Space`
- Fuzzy search with exact, prefix, substring, near-match, typo-tolerant, and multi-word matching
- Ranking boosts based on built-in rules, file type, path rules, extension rules, and recent use
- Background indexing of fixed local drives
- Folder indexing plus configurable file-type indexing, with optional `Include all file types`
- Excluded path support so unwanted locations stay out of indexing and watchers
- Real-time filesystem updates with `ReadDirectoryChangesW` plus periodic full reindex support
- File and folder launching with keyboard-first navigation
- `Shift` + `Enter` to open the containing folder of the selected result
- Shell context menu access from search results
- Inline calculator with functions such as `sqrt`, `sin`, `pi`, and `e`
- Custom commands in classic keyword mode and slash palette mode
- Save/Open dialog folder navigation mode
- System tray menu with rebuild, settings, index statistics, help, and exit actions
- Theme support and settings pages for ranking, commands, exclusions, file types, and reindex timing
- Index Statistics tools, including per-extension folder distribution browsing and exclusion workflow
- Startup initialization prompt that temporarily blocks typing until the first index is ready
- Built-in update checks with release notes, checksum verification, silent installer handoff, and relaunch

## How To Use Listo

### 1. Open the launcher

- Press `Ctrl` twice quickly, or press `Ctrl` + `Space`
- If Listo is still initializing on first launch, wait a few seconds for the first index to finish
- Press the same shortcut again to hide it
- Press `Escape` to clear the query, then press it again on an empty box to close it

### 2. Search and launch

- Start typing part of a file or folder name
- Press `Up` and `Down` to move through results
- Press `Enter` to open the selected result
- Press `Shift` + `Enter` to open the selected result's containing folder
- Right-click a result to open the Windows shell context menu

Examples:

- `computer notes`
- `my backups`
- `computr`

### 3. Use filters

- `c ` searches only drive `C:`
- `cf ` searches folders only on drive `C:`
- `<space>` before a query searches folders only across all drives
- `ss ` shows shortcuts and app-style launcher entries
- `.pdf ` filters to a file extension

### 4. Use commands

- Type `/` to open the command palette
- Type `/keyword args` to run a command directly
- Type `keyword args` for classic command mode when a command is configured that way
- Press `Backspace` on empty input to exit command mode

Default examples:

- `r dir`
- `ping 8.8.8.8`
- `/notepad hosts`

### 5. Use the built-in calculator

Type a math expression directly in the launcher:

- `2+3*4`
- `sqrt(16)`
- `sin(pi/2)`

Press `Enter` on the calculator result to copy the value to the clipboard.

### 6. Use Listo inside Save/Open dialogs

When a Save or Open dialog is focused, Listo can switch into folder-selection mode:

- results are limited to folders
- selecting a folder changes the host dialog to that location
- `Backspace` on empty input exits dialog mode

### 7. Manage settings and updates

- Open the tray menu for `Settings...`, `Index Statistics...`, `Help & About...`, `Rebuild Index`, and more
- Use `Settings > General` to control update checks and ranking-related options
- Use `Settings > Commands`, `Excluded`, `File Types`, and `Reindex` to tune behavior
- Use `Help & About...` or `Settings > General` to check for updates manually

## Notes

- This repository is the public distribution endpoint for binaries, release notes, and update metadata.
- The Listo source code is not hosted in this repository.
- In-app updates read [`latest.json`](https://raw.githubusercontent.com/Saif-A/listo/main/latest.json) to discover the current stable installer.

## Links

- Public repo: [https://github.com/Saif-A/listo](https://github.com/Saif-A/listo)
- Releases: [https://github.com/Saif-A/listo/releases](https://github.com/Saif-A/listo/releases)
- Latest manifest: [latest.json](https://raw.githubusercontent.com/Saif-A/listo/main/latest.json)

Attribution: Saif A.
