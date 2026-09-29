<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/readme-logo-light.svg">
    <img alt="Howse" src="assets/readme-logo-dark.svg" width="240">
  </picture>
</p>

<p align="center"><strong>코딩 에이전트를 한 팀으로.</strong></p>

<p align="center">Codex, Claude Code 등 코딩 에이전트가 역할을 맡고, 스레드 안에서 일을 넘기고, 사람이 정할 일은 사람에게 묻는 데스크톱 앱입니다.</p>

<p align="center">
  <a href="https://howse-delta.vercel.app/ko/">웹사이트</a> ·
  <a href="https://howse-delta.vercel.app/ko/docs/">문서</a> ·
  <a href="CHANGELOG.md">변경 이력</a> ·
  <a href="https://github.com/swimit-io/howse/issues/new/choose">문제 신고</a> ·
  <a href="README.md">English</a>
</p>

<p align="center">
  <img alt="Howse에서 에이전트들이 스레드로 협업하는 실제 앱 화면" src="assets/hero-1600.webp" width="960">
</p>

## 다운로드

**Howse 0.10.0을 macOS(Apple Silicon·Intel)와 Windows x64 베타로 제공합니다.** macOS 설치 파일은 Apple Developer ID로 서명하고 Apple 공증을 받았습니다. Windows 설치 파일은 아직 코드 서명이 없어 실행할 때 Windows 보안 경고가 나타날 수 있습니다.

[최신 릴리스 내려받기](https://github.com/swimit-io/howse/releases/latest) · [설치 안내](https://howse-delta.vercel.app/ko/docs/install/)

설치한 뒤에는 Howse가 이 저장소에서 업데이트를 확인합니다. 패치 업데이트는 자동으로 적용되고, 마이너·메이저 업데이트는 앱에서 **업데이트** 버튼을 눌러 적용합니다.

## Howse에서 하는 일

- **역할을 나눕니다.** 개발, 검토 등 역할마다 사용할 에이전트를 정합니다.
- **한 스레드에서 협업합니다.** 에이전트가 작업을 넘기고 결과를 돌려받으며, 대화와 실행 기록이 함께 남습니다.
- **결정과 이유를 이어 갑니다.** 내장된 [Whyve](https://github.com/swimit-io/whyve)가 결정과 그 이유 같은 프로젝트 맥락을 다음 작업에서도 읽을 수 있게 보관합니다.
- **필요한 순간에 참여합니다.** 사람이 결정하거나 승인할 일이 생기면 스레드에서 바로 답합니다.

## 설치 조건

| 항목 | 필요한 것 |
|---|---|
| 컴퓨터 | Apple Silicon 또는 Intel 프로세서 Mac, 또는 64비트 Windows 10·11 PC(베타) |
| 에이전트 | 설치하고 로그인한 에이전트 CLI 하나 이상. 예: Codex CLI 0.154.0 이상, Claude Code CLI 2.1.260 이상 |
| 작업 도구 | 맡길 작업에 필요한 Git, npm 등의 도구 |

Node.js와 Whyve는 앱에 포함되어 있어 따로 설치하지 않아도 됩니다. Gemini CLI, OpenCode, GitHub Copilot CLI, Kimi Code, Qwen Code, Cursor CLI, Antigravity CLI도 쓸 수 있으며, 최소 버전은 [요구사항](https://howse-delta.vercel.app/ko/docs/requirements/)에서 확인하세요. Linux는 지원하지 않습니다.

설치와 첫 프로젝트 설정은 [사용 문서](https://howse-delta.vercel.app/ko/docs/)를 참고하세요.

## 사용과 개인정보

이 저장소는 Howse의 다운로드, 릴리스 노트, 지원을 위한 공개 저장소입니다. 앱 소스 코드는 공개하지 않습니다.

에이전트를 사용하려면 각 CLI 제공사의 계정과 이용 조건을 따라야 합니다. 요청과 에이전트가 읽은 프로젝트 내용은 해당 모델 제공사로 전송될 수 있습니다. 실행 권한과 데이터 처리 범위는 [실행 모드](https://howse-delta.vercel.app/ko/docs/execution-modes/)와 [자주 묻는 질문](https://howse-delta.vercel.app/ko/docs/faq/)에서 확인하세요.

웹사이트에서 소식 알림을 신청할 때 수집하는 정보는 [개인정보 안내](https://howse-delta.vercel.app/ko/privacy/)에 설명되어 있습니다.

## 문제 신고

[문제 신고 양식](https://github.com/swimit-io/howse/issues/new/choose)에 앱 버전, 운영체제와 버전, 사용한 에이전트 CLI와 버전, 재현 방법을 적어 주세요. 공개 이슈이므로 비밀번호, 토큰, 개인 대화, 비공개 프로젝트 파일은 올리지 마세요.
