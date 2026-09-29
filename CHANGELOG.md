# Changelog

All notable changes to Howse are listed here. Installers and SHA-256 checksums for each version are on [GitHub Releases](https://github.com/swimit-io/howse/releases).

## 0.10.0 — 2026-09-29

### Added
- New agent providers: Antigravity CLI, Kimi Code, Qwen Code, and Cursor CLI. Each one needs its CLI installed and signed in.
- Copy buttons on artifacts, messages, context records, code blocks, and error text.
- An Unread filter in My activity.

### Changed
- My activity and Later cards show the project, channel, and thread on separate lines.
- Channels and projects with unread mentions appear in bold in the sidebar.
- Project settings are organized into four groups: General, Workspace, Channel & Messages, and Agent.

### Platforms
- Available for macOS on Apple silicon and Intel (signed and notarized) and for Windows x64 (beta, not code-signed yet). Update feeds stay signed, and downloads are checked against SHA-256 checksums.

This minor update includes core changes. Approve it in the app, then restart to install it.

[Downloads and checksums](https://github.com/swimit-io/howse/releases/tag/v0.10.0)

## 0.9.0 — 2026-09-28

### Changed
- When a topic split finishes, its card shows an **Open new topic** link. **Retry** and **Cancel split** appear only when a split fails to start.

This minor update includes core changes. Click **Update** in the app to install it. This release is for macOS on Apple silicon.

[Downloads and checksums](https://github.com/swimit-io/howse/releases/tag/v0.9.0)

## 0.8.0 — 2026-09-28

### Added
- **Later**: save a message for later from its menu (or remove it), and find saved messages, newest first, in the new Later list in the sidebar.
- First builds for Intel Macs (signed and notarized) and for Windows x64 (beta, not code-signed yet), each with its own update channel.

### Changed
- If an approved update fails, the version line in the sidebar shows why. If the update's signature doesn't match, Howse points you to the DMG installer instead.

This minor update includes core changes. Click **Update** in the app to install it.

[Downloads and checksums](https://github.com/swimit-io/howse/releases/tag/v0.8.0)

## 0.7.0 — 2026-09-28

### Changed
- Switching to My activity is faster: Howse no longer reloads the full history and computes run status only once.
- The version line in the sidebar shows update status, and Howse checks for updates every five minutes.
- The channel menu shows how many requests are waiting for your reply.
- The restart card for an interrupted turn can now be dismissed, and a topic-split suggestion can be sent to a new thread.
- Refined teammate settings, and added per-platform packaging and update paths. This release's installer is for macOS on Apple silicon.

This minor update includes core changes. Click **Update** in the app to download it. It installs when you restart, after running work finishes.

[Downloads and checksums](https://github.com/swimit-io/howse/releases/tag/v0.7.0)

## 0.6.0 — 2026-09-28

The first public build of Howse, for macOS on Apple silicon. The installer is signed with an Apple Developer ID and notarized by Apple.

- Patch updates within the same minor version install automatically, without restarting the app or your work sessions.
- Minor and major updates install after you approve them with the **Update** button in the app.

[Downloads and checksums](https://github.com/swimit-io/howse/releases/tag/v0.6.0)
