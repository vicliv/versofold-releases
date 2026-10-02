# VersoFold 0.4.1

October 2, 2026 · macOS 13 or later (Apple silicon and Intel) · Linux x64

This patch fixes problems across agents, editing, recovery, navigation, figures and exports.

## Agents

- The editor and PDF reader use the same agent choices and shared conversation controls, including connected Claude Code. Context and suggested prompts still follow what you are working on.
- Claude model defaults follow the current model aliases, and Settings lets you choose which models appear in the menu.
- Fixes improve connected-agent sessions, history, usage reporting, pending actions and project context.

## Saving and recovery

- File saves keep edits made while a save is in progress. Closing tabs, renaming files and switching projects preserve pending work and handle conflicts more reliably.
- Offline recovery continues saving later edits and retains recovered drafts until the host confirms they were saved. Damaged recovery records cannot replace valid document text.
- History restores check for changes made after the preview. Project settings and workspace changes are handled in sequence.
- Creating a file cannot overwrite another file created at the same moment. Invalid file-operation paths cannot target the whole project folder.

## Data and exports

- CSV and JSON imports preserve columns and values more reliably, including quoted fields and line endings. Missing numeric values stay missing instead of becoming zero.
- Figures, tables and transformations handle missing data consistently; formulas report unknown columns.
- Figure PNG exports respect resolution and transparency. Archive exports handle unusual filenames and report incomplete exports instead of returning a partial download.

## Navigation and controls

- Slow file loading cannot override your latest tab selection. Empty folders offer the file-creation menu.
- Keyboard shortcuts respect text composition and actions already handled by a field. Escape cancels deadline edits without saving them.
- Deadline validation, ordering and countdowns agree across the workspace. The outline handles multiline and nested LaTeX headings.
- Search, folder browsers, project forms, comments and settings better preserve current input when requests finish late or fail.

## Downloads

The macOS DMGs contain the Developer ID-signed, Apple-notarized app. Open the DMG for your Mac and drag VersoFold into Applications. Existing installs update from within the app.

On Ubuntu or Debian, install the `.deb` with `sudo apt install ./VersoFold-0.4.1-x64.deb`. On other distributions, make the AppImage executable and run it (Ubuntu also needs `sudo apt install libfuse2t64` for AppImages). The Linux packages are not signed.

| Computer | Installer | SHA-256 |
| --- | --- | --- |
| Mac, Apple silicon | `VersoFold-0.4.1-arm64.dmg` | `a0df7d0910ea30eb2fda14d77e49ba8bd3f9662fa9230a88ff69495d54fefd2f` |
| Mac, Intel | `VersoFold-0.4.1-x64.dmg` | `1e7c3080eab506720eaa61716cefc52df284c80ff20cd7737c7ec2766bfaa811` |
| Linux x64, Ubuntu/Debian | `VersoFold-0.4.1-x64.deb` | `d6a9b297587ccd700e64fa06256333bbaf57046aa78aab1562c38622fe5f8a62` |
| Linux x64, other | `VersoFold-0.4.1-x64.AppImage` | `d3d1c18546ebf10a1b6e4d351e923f5f87a696023ccd748201b20fe8ba0cb3c1` |

The ZIP files, blockmaps, `latest-mac.yml` and `latest-linux.yml` support in-app updates.

The official desktop app remains free to use under the [VersoFold Desktop Software License](https://versofold.com/versofold-license.txt). Your documents remain yours; see the [third-party notices](https://versofold.com/third-party-notices.txt) for included components.
