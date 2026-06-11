# Listo

Listo is a fast native Windows launcher for apps, files, folders, Windows settings, calculator expressions, and custom commands. Press `Ctrl + Space`, type what you need, and open it without leaving the keyboard.

Listo indexes folders plus important file types by default. You can also enable `Include all file types` in Settings when you want broader coverage and accept the extra memory cost.

## Quick Start

1. Open [the latest release page](https://github.com/Saif-A/listo/releases/latest) and download `Listo_Setup_1.0.72.exe`.
2. Run the installer.
3. Launch Listo from the Start Menu if it does not start automatically.
4. Press `Ctrl + Space` or double-tap `Ctrl` to show the launcher.
5. Type part of a file, folder, app, or setting name.
6. Press `Enter` to open the selected result, or `Shift + Enter` to open its containing folder.

## Features

### Fast Launcher

- Keyboard-first activation with `Ctrl + Space` or double-tap `Ctrl`.
- Fast native Win32 interface designed for low-latency search.
- Per-monitor launcher placement that opens on the screen under the current mouse pointer, not the last focused window, remembers safe position per display, and recenters if saved coordinates would place any part of the search box off-screen.
- First-install bilingual launcher tutorial starts after initial indexing and can be replayed later.
- Keyboard navigation for results, filters, command modes, and window hiding.
- Shell context menu support from search results.

### Search And Ranking

- Fuzzy search across indexed files, folders, apps, shortcuts, Windows settings, and Control Panel items.
- Exact, prefix, substring, near-match, and typo-tolerant matching.
- Multi-word matching with word-boundary preference and compact fallback.
- Smart scoring with file type, path, extension, exact-match, depth, and recent-use boosts.
- Configurable built-in scoring rules, path boost rules, and extension boost rules.

### Filters

- Type `c ` to search drive `C:` only. The same pattern works for other local drives.
- Type `cf ` to search folders on drive `C:` only.
- Start with a space to search folders only across all drives.
- Type `.pdf `, `.docx `, or any extension plus space to filter by file type.
- Type `ss ` to search shortcuts and app-style entries.
- Press `Backspace` on empty input to clear the active filter or mode.

### Interactive Tutorial

- Runs automatically once on a genuine first installation after initial indexing.
- Supports English and Arabic with a language switch at every step.
- Provides Previous, Next, and Exit controls.
- Uses black slide details and blue highlighted input prompts at the same font size, with a slower typing cadence for launcher shortcut prefixes.
- Demonstrates separate application, file, and Windows Settings searches, leading-space folder-only search, drive-only search for any result type, other filters, four calculator expressions, command palette, and keyboard navigation without opening files or executing commands.
- Includes short promotion slides showing where to enable the optional Standup Timer and Resource Monitor.
- Can be replayed from the first idle-help item, the Ctrl+Space introduction notification, Help/About, or the tray menu.

### Indexing

- Background fixed-drive indexing that keeps the launcher responsive.
- Folder indexing is always enabled.
- Extension-list indexing by default for lower memory usage.
- Optional `Include all file types` mode for full file coverage.
- Visible excluded-path settings with portable environment-variable rules.
- Exclusion tester that explains which rule would skip a path.
- `ReadDirectoryChangesW` watchers for live filesystem updates.
- Optional periodic full reindex safety net for missed watcher events, disabled by default.
- Drive-disconnect handling that clears stale indexed results from removed drives.
- Startup initialization prompt while the first index is being prepared.
- No administrator privileges required for normal indexing.

### File Dialog Navigation

- Activating Listo while a Save/Open dialog is focused enters folder-selection mode.
- Results are locked to folders so you can navigate the dialog quickly.
- The prompt shows the target app and current dialog folder when available.
- Press `Tab` to cycle already-open File Explorer windows and use an Explorer path as the dialog folder.
- Accepted folder selections are added to recent history for future ranking.

### Calculator And Commands

- Inline calculator for expressions such as `2+2`, `sqrt(16)`, or `sin(pi/2)`.
- Press `Enter` on a calculator result to copy it to the clipboard.
- Custom commands with classic `keyword arguments` mode.
- Slash command palette with `/`, `/keyword`, and `/keyword arguments`.
- Optional silent and run-as-admin command execution settings.

### Settings And Tools

- Settings tabs for General, Path Boost, Extension Boost, Commands, Excluded paths, File Types, Standup, Taskbar Monitor, and Settings Management.
- Settings Management actions to export saved settings, validate and import a Listo INI file, or restore all defaults.
- `Escape` closes Settings through the Cancel path without applying unsaved edits.
- Theme support with Dark, Light, and System options.
- General settings include update checks, built-in scoring rules, and auto-reindex timing; auto-reindex defaults to disabled.
- Optional transparent taskbar monitor readings with network speed, CPU usage, memory usage, optional CPU frequency, enable/disable, monitored-adapter selection, saved-adapter fallback, and main-monitor or all-monitor taskbar display. New installations leave the taskbar monitor disabled and scoped to the main monitor by default.
- Index Statistics window with extension summaries.
- Folder distribution view for a selected extension.
- Exclude folders directly from the distribution workflow.
- Help and About window with tutorial replay, shortcuts, usage notes, version, author, and update controls.
- System tray menu for Show, Rebuild Index, Index Statistics, Settings, Theme, tutorial replay, Help/About, and Exit.
### Updates

- Automatic update checks on launch, enabled by default.
- Manual `Check update now` action in Help/About and Settings.
- Silent automatic failures so startup is not interrupted.
- Release notes shown only when a newer version is available.
- Installer download with checksum verification.
- Silent installer handoff and relaunch after update.

### Standup Reminder

- Optional standup reminder, disabled by default.
- Configurable work interval and break duration.
- Selectable `Enforced break mode` or non-blocking `Break reminder mode`, with enforced mode as the default.
- Default-off idle detection option that pauses the normal interval while the computer is idle.
- Enforced mode uses a full-screen greenish reminder overlay on every connected display.
- Reminder mode shows a Listo notification for 10 seconds without blocking the screen or keyboard.
- Remaining-time counter on each break overlay.
- Sleep is treated as break time, so waking Windows starts a fresh work interval and hides any active reminder UI.
- Optional enforced-mode 15-second pre-break notification, disabled by default, using the shared Listo notification style.
- One-time `Delay for 2 minutes` action on the first enforced-mode pre-break notification; reminder mode skips the pre-break notice.
- Subtle Windows sounds when a break starts and ends.

## Shortcuts

| Shortcut | Action |
|---|---|
| `Ctrl + Space` | Show or hide Listo |
| `Ctrl` + `Ctrl` | Show or hide Listo |
| `Ctrl + Shift + Space` | Rebuild the index |
| `Enter` | Open the selected result |
| `Shift + Enter` | Open the containing folder |
| `Up` / `Down` | Move through results |
| `Escape` | Clear the query, then hide the launcher if already empty |
| `Backspace` on empty input | Clear filter, exit folder mode, or exit command mode |

## Notes

- This repository is the public distribution endpoint for binaries, release notes, and update metadata.
- The Listo source code is not hosted in this repository.
- In-app updates read [latest.json](https://raw.githubusercontent.com/Saif-A/listo/main/latest.json) to discover the current stable installer.

## Links

- Latest release: [https://github.com/Saif-A/listo/releases/latest](https://github.com/Saif-A/listo/releases/latest)
- Public repo: [https://github.com/Saif-A/listo](https://github.com/Saif-A/listo)
- All releases: [https://github.com/Saif-A/listo/releases](https://github.com/Saif-A/listo/releases)
- Latest manifest: [latest.json](https://raw.githubusercontent.com/Saif-A/listo/main/latest.json)

Attribution: Saif A.
