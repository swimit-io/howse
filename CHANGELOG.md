# Changelog

All notable changes to Howse are listed here. Installers and SHA-256 checksums for each version are on [GitHub Releases](https://github.com/swimit-io/howse/releases).

## 0.44.0 — 2026-10-23

### What's new
- Find colleagues on a paired desktop, mention them in your message, and hand off work with results returned to the conversation. Desktop-to-desktop collaboration requires online devices on the same account, device approval, and a compatible server policy.
- Give linked folders your own display names. Paths missing on this computer stay linked with a warning, including folders belonging to another operating system.
- Open a saved artifact’s storage folder directly from its preview, or show a working-folder file in your file manager.

### Changes
- The message composer grows with your text up to 60% of the window height. Keyboard navigation keeps the selected mention role visible.
- Project registration preserves other devices’ folder links and shows clearer locations when a project move conflicts.
- Saved output has stronger integrity and storage checks. Automatic artifact collection remains unavailable.

### 새로운 기능
- 연결된 데스크톱의 동료를 찾아 작성창에서 멘션하고, 작업을 인계해 대화로 결과를 돌려받을 수 있습니다. 같은 계정의 온라인 기기, 기기 승인과 호환되는 서버 정책이 필요합니다.
- 연결 폴더에 원하는 표시 이름을 붙일 수 있습니다. 다른 운영체제의 경로를 포함해 이 컴퓨터에 없는 폴더도 경고와 함께 연결을 유지합니다.
- 아티팩트 미리보기에서 저장 폴더를 바로 열거나, 작업 폴더 파일을 파일 관리자에서 찾을 수 있습니다.

### 변경 사항
- 메시지 입력창이 내용에 따라 창 높이의 60%까지 늘어납니다. 멘션 역할을 키보드로 고르면 선택 항목이 보이도록 유지합니다.
- 프로젝트 등록 시 다른 기기의 폴더 연결을 보존하고, 프로젝트 이동이 충돌하면 해당 위치를 더 명확하게 표시합니다.
- 결과물 저장의 무결성과 용량 확인을 강화했습니다. 자동 아티팩트 수거는 제공하지 않습니다.

Platforms: macOS Apple silicon / Intel; Windows x64 (unsigned beta).

지원 플랫폼: macOS Apple Silicon·Intel, Windows x64(미서명 베타).

[Downloads and checksums / 다운로드 및 체크섬](https://github.com/swimit-io/howse/releases/tag/v0.44.0)


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
