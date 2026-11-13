# Changelog

All notable changes to Howse are listed here. Installers and SHA-256 checksums for each version are on [GitHub Releases](https://github.com/swimit-io/howse/releases).

## 0.59.0 — 2026-11-13

## What's new
- Choose session handling per agent tool: keep sessions, refresh after idle time, or start fresh when completed work and recovery conditions allow.
- Address specific teammate roles and distinguish recipients from reference-only roles. Fresh-session recovery prioritizes role focus and active records.
- Read managed documents by contents, section or line range; search a fixed revision and apply sequential partial edits with idempotent revisions.

## Changes
- Preserve recovery pages, inbox delivery progress and pending hints more accurately; reduce recovery stack growth and repeated context output.
- Improve collaboration tool input and checkpoint error guidance, and restore bottom detection and automatic following after fractional scrolling.
- Add cookie-free website visit statistics with updated privacy notices.

## 새로운 기능
- 실행 도구별로 세션 유지, 유휴 후 교체, 복구 조건을 충족하면 매번 새 세션 시작을 선택합니다.
- 동료의 대상 역할과 수신·참조 역할을 구분하고 새 세션 복구에서 역할 초점과 활성 기록을 우선 전달합니다.
- 산출물의 목차·절·줄 범위를 읽고 고정 개정에서 검색하며, 순차 부분 수정과 멱등 개정을 지원합니다.

## 변경 사항
- 복구 페이지와 inbox 전달 진행·대기 표식을 보존하고 복구 스택 증가와 반복 컨텍스트 출력을 줄입니다.
- 협업 도구 입력·점검 오류 안내와 소수점 스크롤 후 하단 표시·자동 추적을 개선합니다.
- 사이트에 쿠키 없는 방문 통계를 추가하고 개인정보 안내를 갱신했습니다.

Platforms: macOS Apple Silicon / Intel (signed and notarized); Windows x64 (unsigned beta).
지원 플랫폼: macOS Apple Silicon·Intel(서명·공증), Windows x64(미서명 베타).

[Downloads and checksums / 다운로드 및 체크섬](https://github.com/swimit-io/howse/releases/tag/v0.59.0)

## 0.58.0 — 2026-11-11

## What's new
- Add common agent instructions shared across all projects and teammates. Saved changes apply from the next run, with explicit priorities for protocol, persona, project and role instructions.
- Supported Claude Code and Codex sessions receive linked-workspace rules when Howse observes access, reducing unused instructions. The first access can precede rule delivery; other providers retain prompt-time delivery.

## Changes
- Record workspace rule delivery receipts and measurements to distinguish supplied rules from pending rules.

## 새로운 기능
- 모든 프로젝트와 동료에게 적용하는 에이전트 공통지침을 추가했습니다. 저장한 변경은 다음 실행부터 적용되며 프로토콜·페르소나·프로젝트·역할 지침의 우선순위를 명시합니다.
- 지원되는 Claude Code·Codex 세션에서 접근을 관찰한 연결 작업영역의 규칙을 공급해 사용하지 않는 지침을 줄입니다. 첫 접근이 규칙 공급보다 앞설 수 있으며 다른 프로바이더는 시작 프롬프트 공급을 유지합니다.

## 변경 사항
- 작업영역별 규칙 공급 영수증과 계측을 기록해 공급한 규칙과 대기 중인 규칙을 구분합니다.

Platforms: macOS Apple Silicon / Intel (signed and notarized); Windows x64 (unsigned beta).
지원 플랫폼: macOS Apple Silicon·Intel(서명·공증), Windows x64(미서명 베타).

[Downloads and checksums / 다운로드 및 체크섬](https://github.com/swimit-io/howse/releases/tag/v0.58.0)

## 0.57.0 — 2026-11-11

## Changes
- In the channel list, a message's Work details and Forwarded messages now appear as buttons that open the thread at that message, instead of expanding in place.
- Agents in threads that keep collaboration records no longer receive duplicated text: collaboration guidance comes only from their system instructions, and messages supplied directly to a freshly recovered session are no longer repeated.

## 변경 사항
- 채널 목록에서 메시지의 작업 상세와 전달한 원문을 그 자리에서 펼치지 않고, 누르면 스레드의 해당 메시지로 이동하는 버튼으로 표시합니다.
- 협업 기록을 남기는 스레드의 에이전트가 같은 내용을 중복해서 받지 않습니다. 협업 안내는 시스템 지침에서만 공급하고, 새로 복구한 세션에 직접 공급한 메시지 본문도 반복하지 않습니다.

Platforms: macOS Apple Silicon / Intel (signed and notarized); Windows x64 (unsigned beta).
지원 플랫폼: macOS Apple Silicon·Intel(서명·공증), Windows x64(미서명 베타).

[Downloads and checksums / 다운로드 및 체크섬](https://github.com/swimit-io/howse/releases/tag/v0.57.0)

## 0.56.0 — 2026-11-10

## Changes
- Deliver the final report of a retried or continued turn in threads that keep collaboration records, instead of rejecting it as an identity conflict.

## 변경 사항
- 협업 기록을 남기는 스레드에서 재시도되거나 이어진 턴의 최종 보고를 신원 충돌로 거부하지 않고 정상적으로 전달합니다.

Platforms: macOS Apple Silicon / Intel (signed and notarized); Windows x64 (unsigned beta).
지원 플랫폼: macOS Apple Silicon·Intel(서명·공증), Windows x64(미서명 베타).

[Downloads and checksums / 다운로드 및 체크섬](https://github.com/swimit-io/howse/releases/tag/v0.56.0)

## 0.55.0 — 2026-11-09

## What's new
- New macOS threads keep topic-level collaboration records in local files, and each role resumes from the position it last read. Existing threads and the Windows app keep the shared snapshot behavior.

## Changes
- Keep Claude runs active until their background tasks finish, and show the number of background tasks in the run bar.
- Show **Preparing the report** while a turn that keeps collaboration records settles its result.
- Apply the message jump highlight to the header as well, and keep the jump-to-bottom button readable on hover.
- Route threads opened by agents the same way as threads opened by people.
- Reduce context handling work on long conversation histories.

## 새로운 기능
- macOS의 새 스레드는 주제별 협업 기록을 로컬 파일로 남기고, 각 역할은 마지막으로 읽은 위치부터 이어갑니다. 기존 스레드와 Windows 앱은 공유 스냅샷 방식을 유지합니다.

## 변경 사항
- Claude 실행을 백그라운드 작업이 끝날 때까지 유지하고 실행바에 백그라운드 작업 개수를 표시합니다.
- 협업 기록을 남기는 턴이 결과를 정리하는 동안 **보고 준비 중**으로 표시합니다.
- 메시지 이동 강조를 헤더까지 적용하고 하단 이동 버튼의 hover 대비를 유지합니다.
- 에이전트가 여는 스레드도 사람이 여는 스레드와 같은 방식으로 전달합니다.
- 긴 대화 이력에서 컨텍스트 처리 부담을 줄였습니다.

Platforms: macOS Apple Silicon / Intel (signed and notarized); Windows x64 (unsigned beta).
지원 플랫폼: macOS Apple Silicon·Intel(서명·공증), Windows x64(미서명 베타).

[Downloads and checksums / 다운로드 및 체크섬](https://github.com/swimit-io/howse/releases/tag/v0.55.0)

## 0.54.2 — 2026-11-06

## Changes
- Extend the focused message outline through its header so the entire selected message stays visible.

## 변경 사항
- 선택한 메시지의 강조 테두리가 헤더까지 이어지도록 개선했습니다.

Platforms: macOS Apple Silicon / Intel (signed and notarized); Windows x64 (unsigned beta).
지원 플랫폼: macOS Apple Silicon·Intel(서명·공증), Windows x64(미서명 베타).

[Downloads and checksums / 다운로드 및 체크섬](https://github.com/swimit-io/howse/releases/tag/v0.54.2)

## 0.54.1 — 2026-11-04

## What's new
- Keep attached artifact cards in one row and expand the remaining cards with a count button; collapse them again without losing your reading position.

## Changes
- Return to the bottom of a channel or thread with a dedicated button, and resume following new content when reaching the bottom.
- Preserve reading position during layout changes and keep nested code-block scrolling independent.
- Use singular and plural English labels for remaining artifact counts.

## 새로운 기능
- 메시지의 첨부 아티팩트 카드를 한 줄로 접고 남은 개수 버튼으로 펼칠 수 있습니다. 다시 접을 때도 읽던 위치를 유지합니다.

## 변경 사항
- 채널·스레드의 하단 이동 버튼으로 최신 대화로 돌아가며 맨 아래에 도달하면 새 내용 따라보기를 재개합니다.
- 레이아웃이 바뀔 때 읽던 위치를 유지하고 코드 블록 안의 스크롤을 분리합니다.
- 아티팩트 더보기 영어 안내의 단수·복수를 구분합니다.

Platforms: macOS Apple Silicon / Intel (signed and notarized); Windows x64 (unsigned beta).
지원 플랫폼: macOS Apple Silicon·Intel(서명·공증), Windows x64(미서명 베타).

[Downloads and checksums / 다운로드 및 체크섬](https://github.com/swimit-io/howse/releases/tag/v0.54.1)

## 0.54.0 — 2026-11-04

## What's new
- Explicitly ask an agent to open a new thread in another project's channel. The new work uses the destination project while explicit artifact attachments come from the sender's workspace. Destination, content and recipients require your instruction or approval.

## 새로운 기능
- 에이전트에게 다른 프로젝트 채널의 새 스레드 개시를 명시적으로 요청할 수 있습니다. 새 작업은 대상 프로젝트에서 실행하며 명시적으로 첨부한 아티팩트는 보내는 작업 폴더에서 가져옵니다. 대상·내용·수신자에 대한 사용자 지시나 승인이 필요합니다.

Platforms: macOS Apple Silicon / Intel (signed and notarized); Windows x64 (unsigned beta).
지원 플랫폼: macOS Apple Silicon·Intel(서명·공증), Windows x64(미서명 베타).

Includes 0.53.0 artifact saving and channel reaction fixes. Restart manually after current work finishes. Cloud integration, mobile releases, review apps and server redeployment are excluded.
0.53.0의 아티팩트 저장 통합과 채널 반응 수정을 포함합니다. 진행 중인 작업이 끝난 뒤 수동으로 재시작하세요. 클라우드 통합·모바일 출시·심사용 앱·서버 재배포는 제외합니다.

[Downloads and checksums / 다운로드 및 체크섬](https://github.com/swimit-io/howse/releases/tag/v0.54.0)

## 0.53.0 — 2026-11-04

## What's new
- Save text, Markdown and HTML documents, images and PDFs from one button at the top of the artifact preview, with format-aware filenames.

## Changes
- Keep channel reactions consistent when opening a thread, using each colleague’s latest run state.

## 새로운 기능
- 아티팩트 미리보기 상단의 공통 저장 버튼으로 텍스트·Markdown·HTML 문서, 이미지와 PDF를 형식에 맞는 파일명으로 내보낼 수 있습니다.

## 변경 사항
- 스레드를 열어도 채널 반응이 동료별 마지막 실행 상태를 일관되게 표시합니다.

Platforms: macOS Apple Silicon / Intel (signed and notarized); Windows x64 (unsigned beta).
지원 플랫폼: macOS Apple Silicon·Intel(서명·공증), Windows x64(미서명 베타).

Restart manually after current work finishes. Cloud integration, mobile releases, review apps, and server redeployment are excluded.
진행 중인 작업이 끝난 뒤 수동으로 재시작하세요. 클라우드 통합·모바일 출시·심사용 앱·서버 재배포는 제외합니다.

[Downloads and checksums / 다운로드 및 체크섬](https://github.com/swimit-io/howse/releases/tag/v0.53.0)

## 0.52.0 — 2026-11-02

## Changes
- Let normally finished turns complete silently when the final response is empty, without an extra provider run or an invented message. An explicitly empty Codex final response no longer reuses earlier progress text as its final result.
- Hide acknowledged past errors in run details as well as the conversation.

- Fix scrolling in project colleague settings and align its colleague order with Teammates (Butler, Clerk, then enabled colleagues by name).

## 변경 사항
- 정상 종료한 턴은 최종 응답이 비어 있어도 추가 실행이나 생성 메시지 없이 조용히 완료됩니다. Codex의 명시적인 빈 최종 응답은 앞선 진행 문장을 최종 결과로 재사용하지 않습니다.
- 확인한 과거 오류를 대화뿐 아니라 실행 상세에서도 숨깁니다.

- 프로젝트 동료 설정의 스크롤을 수정하고, 동료 화면과 같은 순서(집사·기록관·활성 동료 이름순)로 정렬합니다.

Restart manually after current work finishes. Cloud integration, mobile releases, review apps, and server redeployment are excluded.
진행 중인 작업이 끝난 뒤 수동으로 재시작하세요. 클라우드 통합·모바일 출시·심사용 앱·서버 재배포는 제외합니다.

Platforms: macOS Apple Silicon / Intel (signed and notarized); Windows x64 (unsigned beta).
지원 플랫폼: macOS Apple Silicon·Intel(서명·공증), Windows x64(미서명 베타).

[Downloads and checksums / 다운로드 및 체크섬](https://github.com/swimit-io/howse/releases/tag/v0.52.0)

## 0.51.0 — 2026-11-02

## Changes
- Keep channel reactions aligned with each participating agent's latest run in the thread, including retries and continuations. A finished continuation now clears a stale working reaction in the channel list. Reactions inside the thread remain specific to each message.

## 변경 사항
- 채널 반응이 재시도·이어진 실행을 포함해 참여 에이전트별 마지막 실행 상태를 표시합니다. 이어진 실행이 완료됐는데 채널에 작업 중 표시가 남던 문제를 수정했습니다. 스레드 안의 반응은 기존처럼 개별 메시지를 기준으로 표시합니다.

Restart manually after current work finishes. Cloud workspace integration, mobile releases, review apps, and server redeployment are excluded.
진행 중인 작업이 끝난 뒤 수동으로 재시작하세요. 클라우드 작업공간 통합·모바일 출시·심사용 앱·서버 재배포는 포함하지 않습니다.

Platforms: macOS Apple silicon / Intel (signed and notarized); Windows x64 (unsigned beta).
지원 플랫폼: macOS Apple Silicon·Intel(서명·공증), Windows x64(미서명 베타).

[Downloads and checksums / 다운로드 및 체크섬](https://github.com/swimit-io/howse/releases/tag/v0.51.0)

## 0.50.0 — 2026-11-02

## What's new
- Follow each role in a compact, single-line run list. Work status now shows a needs-reply badge and an activity spinner, including when the sidebar is collapsed.
- See each agent's read-only ID in its details. Teammates are sorted by name, with Butler before Clerk.

## Changes
- Keep the run bar, participant panel, and task details aligned on the currently running turn. Waiting only for the context clerk remains visible as active work.
- Retry stopped turns without reviving cancelled sibling or child runs. Superseded sessions remain read-only and no longer leave stale failures in the run bar.
- Keep failed turns in the run controls instead of duplicating interrupted cards in the conversation; hide acknowledged older error cards.
- Finish successfully when an agent has already posted its answer and returns an empty final response.
- Improve mention-chip hover feedback, message role labels, and run-list layout in narrow windows.

## 새로운 기능
- 역할마다 한 줄로 정리된 실행 목록에서 진행 상황을 봅니다. 작업 현황 메뉴에는 응답 필요 뱃지와 실행 스피너가 표시되며, 사이드바를 접어도 확인할 수 있습니다.
- 에이전트 상세에서 읽기 전용 ID를 확인합니다. 동료 목록은 이름순으로 정렬하고 집사는 서기보다 앞에 둡니다.

## 변경 사항
- 실행바·참여자 패널·작업 상세가 현재 진행 중인 턴을 일관되게 표시합니다. 서기의 기록 답변만 기다리는 작업도 실행 중으로 보입니다.
- 중단한 턴을 재시도해도 취소된 형제·하위 실행은 되살리지 않습니다. 교체된 세션은 읽기 전용으로 유지하고 실행바의 과거 실패 표시를 정리합니다.
- 실패한 턴은 실행 목록에서 관리하고 대화에 중복 중단 카드를 만들지 않습니다. 확인한 과거 오류 카드도 숨깁니다.
- 에이전트가 답변을 이미 게시한 뒤 빈 최종 응답을 반환해도 정상 완료합니다.
- 멘션 칩의 호버 표시, 메시지 역할 라벨과 좁은 창의 실행 목록 배치를 다듬습니다.

Restart manually after current work finishes. Cloud workspace integration, mobile releases, review apps, and server redeployment are excluded.
진행 중인 작업이 끝난 뒤 수동으로 재시작하세요. 클라우드 작업공간 통합·모바일 출시·심사용 앱·서버 재배포는 포함하지 않습니다.

Platforms: macOS Apple silicon / Intel (signed and notarized); Windows x64 (unsigned beta).
지원 플랫폼: macOS Apple Silicon·Intel(서명·공증), Windows x64(미서명 베타).

[Downloads and checksums / 다운로드 및 체크섬](https://github.com/swimit-io/howse/releases/tag/v0.50.0)

## 0.49.0 — 2026-10-28

## What's new
- Pick each agent's avatar color from 12 presets or a custom color in its settings; the letter color adjusts automatically for readability. Thread message headers and avatars now stay pinned together within each card.
- Open **Manage** in the run bar as a list above the bar, and expand a running turn to see the progress and background tasks it has posted. A retried or resumed turn continues in the same row.

## Changes
- Close a run as failed once saving works again when its final state could not be saved (for example, a full disk). It no longer stays running or blocks its retry.
- Recover from context reads that need a complete re-read, and reduce duplicate output from MCP context reads.
- Style the project selectors and match the unread toggle height.
- Streamline the built-in agent protocol instructions for messages and roles.

## 새로운 기능
- 에이전트 설정에서 12색 팔레트나 직접 선택으로 아바타 색을 고릅니다. 글자색은 읽기 쉽게 자동으로 맞춥니다. 스레드 메시지 헤더와 아바타는 카드 안에서 함께 고정됩니다.
- 실행바의 **관리**를 바 위에 펼쳐지는 목록으로 열고, 진행 중인 턴을 펼쳐 그 턴이 남긴 진행 기록과 백그라운드 작업을 봅니다. 재시도하거나 재개한 턴은 같은 행에서 이어집니다.

## 변경 사항
- 디스크가 가득 찬 경우처럼 종료 상태를 저장하지 못한 실행을, 저장이 가능해지면 실패로 닫습니다. 더 이상 진행 중으로 남거나 재시도를 막지 않습니다.
- 컨텍스트를 전체 다시 읽어야 하는 경우의 복구를 추가하고, MCP 컨텍스트 조회의 중복 출력을 줄입니다.
- 프로젝트 선택 상자의 스타일을 다듬고 읽지 않음 토글의 높이를 맞춥니다.
- 메시지와 역할에 관한 내장 에이전트 프로토콜 지침을 간결하게 정리합니다.

Restart manually after current work finishes. Mobile source changes are not a mobile release; cloud workspace integration, review apps, and server redeployment are excluded.
진행 중인 작업이 끝난 뒤 수동으로 재시작하세요. 모바일 소스 변경은 모바일 출시를 뜻하지 않으며, 클라우드 작업공간 통합·심사용 앱·서버 재배포는 포함하지 않습니다.

Platforms: macOS Apple silicon / Intel (signed and notarized); Windows x64 (unsigned beta).
지원 플랫폼: macOS Apple Silicon·Intel(서명·공증), Windows x64(미서명 베타).

[Downloads and checksums / 다운로드 및 체크섬](https://github.com/swimit-io/howse/releases/tag/v0.49.0)

## 0.48.0 — 2026-10-27

## What's new
- Filter activity, threads, and Work status by project. Your selection is remembered across these lists.
- Keep Work status on the left while opening a thread beside it.

## Changes
- Keep stopped turns visible in the run bar, with retry and dismissal controls. Dismiss failed or stopped turns in Manage without running them again.

## 새로운 기능
- 내 활동·스레드·작업 현황을 프로젝트별로 좁힙니다. 선택은 이 목록들에서 기억됩니다.
- 작업 현황에서 스레드를 열어도 왼쪽 목록을 유지합니다.

## 변경 사항
- 중단된 턴을 실행바에 남기고 재시도와 확인 처리를 제공합니다. 관리 창에서 실패하거나 중단된 턴을 다시 실행하지 않고 확인 처리할 수 있습니다.

Restart manually after current work finishes. Mobile source changes are not a mobile release; cloud workspace integration, review apps, and server redeployment are excluded.
진행 중인 작업이 끝난 뒤 수동으로 재시작하세요. 모바일 소스 변경은 모바일 출시를 뜻하지 않으며, 클라우드 작업공간 통합·심사용 앱·서버 재배포는 포함하지 않습니다.

Platforms: macOS Apple silicon / Intel (signed and notarized); Windows x64 (unsigned beta).
지원 플랫폼: macOS Apple Silicon·Intel(서명·공증), Windows x64(미서명 베타).

[Downloads and checksums / 다운로드 및 체크섬](https://github.com/swimit-io/howse/releases/tag/v0.48.0)

## 0.47.0 — 2026-10-27

## What's new
- Find threads with active work, pending decisions, and unread final results in Work status. Filter the list and open a thread to continue.
- New project vaults enable assumptions and terms alongside decisions, intents, and documents. Existing vault settings are preserved.

## Changes
- Keep cross-thread handoff runs visible in the session index.
- Open artifact copies with the saved filename and format, while preserving the managed original.
- Accept empty or omitted optional Claude instructions during profile resolution and initialization.
- Avoid subscribing to an empty conversation draft when no thread is selected, and report invalid task timing as an input error.

## 새로운 기능
- 작업 현황에서 진행 중인 스레드, 판단 대기 요청, 읽지 않은 최종 결과를 모아 봅니다. 종류별로 좁히고 스레드를 열어 대화를 이어갈 수 있습니다.
- 새 프로젝트 저장소에서 결정·의도·문서와 함께 가정·용어를 기본 활성화합니다. 기존 저장소 설정은 유지합니다.

## 변경 사항
- 다른 스레드로 인계된 실행도 세션 표시에 유지합니다.
- 아티팩트의 관리 원본을 보존하면서 저장된 파일명과 형식에 맞는 사본 폴더를 엽니다.
- Claude 선택 지침이 비어 있거나 생략돼도 프로필 해석과 초기화를 진행합니다.
- 스레드를 선택하지 않았을 때 빈 대화 초안을 구독하지 않으며, 잘못된 작업 일정은 입력 오류로 안내합니다.

This is a full app update. Restart manually after current work finishes. Cloud workspace features, mobile releases, and server redeployment are not included.
전체 앱 업데이트입니다. 진행 중인 작업이 끝난 뒤 수동으로 재시작하세요. 클라우드 작업공간 기능·모바일 출시·서버 재배포는 포함하지 않습니다.

Platforms: macOS Apple silicon / Intel (signed and notarized); Windows x64 (unsigned beta).
지원 플랫폼: macOS Apple Silicon·Intel(서명·공증), Windows x64(미서명 베타).

[Downloads and checksums / 다운로드 및 체크섬](https://github.com/swimit-io/howse/releases/tag/v0.47.0)

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
