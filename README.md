<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/readme-logo-light.svg">
    <img alt="Howse" src="assets/readme-logo-dark.svg" width="240">
  </picture>
</p>

<p align="center"><strong>AI 코딩 에이전트를 한 팀으로.</strong></p>

<p align="center">Codex와 Claude Code가 역할을 맡고, 스레드 안에서 일을 넘기고, 필요한 순간에 사람의 승인을 받는 Mac 앱입니다.</p>

<p align="center">
  <a href="https://howse-delta.vercel.app/">웹사이트</a> ·
  <a href="https://howse-delta.vercel.app/docs/">문서</a> ·
  <a href="CHANGELOG.md">변경 이력</a> ·
  <a href="https://github.com/swimit-io/howse/issues/new/choose">문제 신고</a>
</p>

<p align="center">
  <img alt="Howse에서 에이전트들이 스레드로 협업하는 실제 앱 화면" src="assets/hero-1600.webp" width="960">
</p>

## 다운로드

**macOS Apple Silicon용 Howse 0.6.0을 공개했습니다.** Apple Developer ID로 서명하고 공증한 설치 파일입니다.

[Howse 0.6.0 다운로드](https://github.com/swimit-io/howse/releases/tag/v0.6.0) · [다운로드 및 설치 안내](https://howse-delta.vercel.app/#get)

## Howse에서 하는 일

- **역할을 나눕니다.** 개발, 검토 등 역할마다 사용할 에이전트를 정합니다.
- **한 스레드에서 협업합니다.** 에이전트가 작업을 넘기고 결과를 돌려받으며 대화와 실행 기록을 함께 남깁니다.
- **결정과 이유를 이어 갑니다.** 내장된 Whyve가 프로젝트 맥락을 다음 작업에서도 읽을 수 있게 보관합니다.
- **필요한 순간에 참여합니다.** 사람이 결정하거나 승인할 일이 생기면 스레드에서 응답합니다.

## 설치 조건

| 항목 | 필요한 것 |
|---|---|
| Mac | macOS를 사용하는 Apple Silicon(arm64) Mac |
| 에이전트 | 설치하고 로그인한 Codex CLI 또는 Claude Code CLI 중 하나 이상 |
| CLI 버전 | Codex CLI 0.154.0 이상 또는 Claude Code CLI 2.1.260 이상 |
| 작업 도구 | 맡길 작업에 필요한 Git, npm 등의 도구 |
| 기본 구성 | Node.js와 Whyve는 앱에 포함되므로 별도 설치가 필요하지 않습니다. |

Intel Mac, Windows, Linux용 빌드는 제공하지 않습니다. 설치와 첫 프로젝트 설정은 [사용 문서](https://howse-delta.vercel.app/docs/)를 참고하세요.

## 사용과 개인정보

이 저장소는 Howse의 **공개 배포·소개·지원용 저장소**입니다. 앱 소스 코드는 공개하지 않습니다.

에이전트를 사용하려면 각 CLI의 계정과 이용 조건을 따라야 합니다. 에이전트가 읽은 요청과 프로젝트 내용은 해당 모델 제공사로 전송될 수 있습니다. 실행 권한과 데이터 처리 범위는 [실행 방식](https://howse-delta.vercel.app/docs/execution-modes/)과 [자주 묻는 질문](https://howse-delta.vercel.app/docs/faq/)에서 확인하세요.

웹사이트 출시 알림 신청 시 수집하는 정보는 [개인정보 안내](https://howse-delta.vercel.app/privacy/)에 설명되어 있습니다.

## 문제 신고

[문제 신고 양식](https://github.com/swimit-io/howse/issues/new/choose)에 앱 버전, macOS 버전, 사용한 CLI와 재현 방법을 알려 주세요. 공개 이슈에는 비밀번호, 토큰, 개인 대화나 비공개 프로젝트 파일을 올리지 마세요.
