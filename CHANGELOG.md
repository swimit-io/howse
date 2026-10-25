# Changelog

All notable changes to Howse are listed here. Installers and SHA-256 checksums for each version are on [GitHub Releases](https://github.com/swimit-io/howse/releases).

## 0.46.0 — 2026-10-25

## Changes
- Keep an open stop or retry confirmation in sync with current execution locks.
- Recover startup when a question record refers to a missing message, without deleting user data.
- Stop all work in a thread even when a pending routing item refers to a missing message.
- Accept empty or omitted optional Codex instructions in native profile validation.

## 변경 사항
- 열린 중단·재시도 확인창에도 현재 실행 잠금을 적용합니다.
- 원본 메시지가 없는 질문 기록이 있어도 사용자 데이터를 삭제하지 않고 시작 복구를 이어갑니다.
- 대기 라우팅 항목의 메시지가 사라져도 스레드 전체 중단이 실패하지 않도록 고쳤습니다.
- Codex 선택 지침이 비어 있거나 생략돼도 native 프로필 검증이 거절하지 않도록 고쳤습니다.

This is a full app update. Restart after current work finishes to apply these fixes. Existing projects and conversations are preserved. No cloud workspace features, mobile store release, or server deployment is included.

전체 앱 업데이트이며 진행 중인 작업이 끝난 뒤 재시작하면 적용됩니다. 기존 프로젝트와 대화는 보존됩니다. 클라우드 작업공간 기능·모바일 스토어·서버 배포는 포함하지 않습니다.

Platforms: macOS Apple silicon / Intel (signed and notarized); Windows x64 (unsigned beta).
지원 플랫폼: macOS Apple Silicon·Intel(서명·공증), Windows x64(미서명 베타).

[Downloads and checksums / 다운로드 및 체크섬](https://github.com/swimit-io/howse/releases/tag/v0.46.0)

## 0.45.0 — 2026-10-24

### What's new
- Follow active agents in a compact run bar above the reply composer. Open Manage to see task states, stop work, or retry in the same session, with confirmation before changes.

### Changes
- Keep more of the conversation in view: empty composing cards are removed, parallel progress is gathered into one collapsed history line, and overlapping runs of one role appear once in the run bar.
- Ask questions while work continues. Agent instructions now require answers to preserve the original task and completion criteria, and focus updates on what you need to understand or decide.
- Reduce repeated context storage in long threads while keeping existing context readable. Earlier inline context is migrated only after its restored content is checked.
- Fold an earlier failed run when a later run of the same role task has completed.

### 새로운 기능
- 답장 입력창 위 한 줄 실행바에서 에이전트 상태를 확인할 수 있습니다. 관리를 열어 작업 상태를 보고 중단하거나 같은 세션에서 재시도할 수 있으며, 변경 전 확인 창을 거칩니다.

### 변경 사항
- 빈 작성 중 카드를 없애고 병렬 진행 기록을 접힌 한 줄로 모아 대화를 더 넓게 볼 수 있습니다. 한 역할의 실행이 겹쳐도 실행바에는 한 번 표시합니다.
- 작업 중 질문에도 원래 작업과 완료 기준을 보존하면서 답하고, 이해나 결정에 필요한 내용을 중심으로 안내하도록 에이전트 지침을 개선했습니다.
- 긴 스레드에서 접수 컨텍스트의 반복 저장을 줄였습니다. 기존 컨텍스트는 계속 읽을 수 있으며, 이전 형식은 복원 내용이 일치하는지 확인한 뒤 이전합니다.
- 같은 역할 작업의 후속 실행이 완료되면 앞선 실패 실행을 접어 표시합니다.

Platforms: macOS Apple silicon / Intel (signed and notarized); Windows x64 (unsigned beta). No mobile store or server deployment is included.

지원 플랫폼: macOS Apple Silicon·Intel(서명·공증), Windows x64(미서명 베타). 모바일 스토어·서버 배포는 포함하지 않습니다.

[Downloads and checksums / 다운로드 및 체크섬](https://github.com/swimit-io/howse/releases/tag/v0.45.0)


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
