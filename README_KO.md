# [AitoEarn: 1인 기업(OPC)을 위한 AI 콘텐츠 마케팅 에이전트](https://aitoearn.ai)

<a href="https://trendshift.io/repositories/20785" target="_blank"><img src="https://trendshift.io/api/badge/repositories/20785" alt="yikart%2FAiToEarn | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>

[![GitHub stars](https://img.shields.io/github/stars/yikart/AiToEarn?color=fa6470)](https://github.com/yikart/AiToEarn/stargazers)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Required Node.JS 20.18.x](https://img.shields.io/static/v1?label=node&message=20.18.x&logo=node.js&color=3f893e)](https://nodejs.org/about/releases)

한국어 | [简体中文](README.md) | [English](README_EN.md) | [日本語](README_JA.md)

**Monetize · Publish · Engage · Create — 올인원 플랫폼.**

AiToEarn는 **AI 자동화**를 통해 OPC(1인 기업), 크리에이터, 브랜드, 기업이 전 세계 주요 플랫폼에서 콘텐츠를 만들고, 배포하고, 수익화할 수 있도록 돕습니다.

지원 채널:
Douyin, Xiaohongshu(Rednote), Kuaishou, Bilibili, TikTok, YouTube, Facebook, Instagram, Threads, Twitter(X), Pinterest, LinkedIn

## 🚀 AiToEarn 빠르게 시작하기 (5가지 방법)

| 방법 | 대상 | 배포 필요 여부 |
|------|------|----------------|
| [① 웹사이트에서 바로 사용](#use-web) | 모든 사용자 | ❌ 불필요 |
| [② OpenClaw에서 사용](#use-in-openclaw) | OpenClaw 사용자 | ❌ 불필요 |
| [③ Claude / Cursor / 기타 AI 도구에서 사용](#use-in-claude) | AI 도구 사용자 | ❌ 불필요 |
| [④ Docker 원클릭 배포](#use-docker) | 셀프호스팅하려는 팀 | ✅ 서버 필요 |
| [⑤ 소스코드로 개발](#use-source) | 개발자 | ✅ 개발 환경 필요 |

> 💡 **방법 ②③④는 먼저 API Key가 필요합니다.** [API Key 받는 방법](#get-api-key)을 먼저 확인하세요.

## 최신 소식

- **2026-04-20**: OpenClaw에서 AiToEarn 수익화 워크플로를 직접 받아 실행할 수 있도록 지원 추가.
- **2026-03-26**: [2.1 버전](https://www.aitoearn.ai/) — 콘텐츠 마켓플레이스 출시, OpenClaw 지원 추가, MCP 프로토콜 지원 추가.
- **2026-02-07**: [1.8.0 버전](https://www.aitoearn.ai/) — 오프라인 매장 홍보 솔루션 추가. 식당, 소매점, 숙박업, 뷰티, 피트니스 등 다양한 오프라인 업종 지원.
- **2025-12-15**: “All In Agent” 시작. 콘텐츠 자동 생성/배포를 지원하는 슈퍼 AI 에이전트 추가. [v1.4.3](https://github.com/yikart/AiToEarn/releases/tag/v1.4.3)
- **2025-11-28**: 앱 내 자동 업데이트 지원. 축약, 확장, 이미지 생성, 영상 생성, 태그 생성 등 다양한 AI 기능 추가. [v1.4.0](https://github.com/yikart/AiToEarn/releases/tag/v1.4.0)
- **2025-11-12**: 첫 오픈소스 완전 사용 가능 버전. [v1.3.2](https://github.com/yikart/AiToEarn/releases/tag/v1.3.2)
- **2025-09-16**: 첫 글로벌 버전, Facebook/Instagram/Threads/Twitter/YouTube/TikTok/Pinterest 지원 추가. [v1.0.18](https://github.com/yikart/AiToEarn/releases/tag/v1.0.18)
- **2025-02-26**: 첫 오픈소스 릴리스, Xiaohongshu/Douyin/Kuaishou/WeChat Channels 원클릭 발행 초기 구현. [v0.1.1](https://github.com/yikart/AiToEarn/releases/tag/v0.1.1)

<details>
  <summary><h2 style="display:inline;margin:0">목차</h2></summary>

  <br/>

  1. [AiToEarn 빠르게 시작하기 (5가지 방법)](#-aitoearn-빠르게-시작하기-5가지-방법)
  2. [최신 소식](#최신-소식)
  3. [핵심 기능](#핵심-기능)
  4. [API Key 받는 방법](#get-api-key)
  5. [기여 가이드](#기여-가이드)
  6. [문의](#문의)
  7. [추천](#추천)
</details>

## 핵심 기능

AiToEarn는 크리에이터의 전체 수익화 흐름을 중심으로 4가지 핵심 Agent 기능을 제공합니다:

> **Monetize · Publish · Engage · Create**

---

### 💰 Monetize — 콘텐츠 수익화

AiToEarn의 가장 중요한 목표는 **모든 크리에이터가 콘텐츠로 수익을 낼 수 있도록 돕는 것**입니다.

크리에이터는 플랫폼에서 콘텐츠를 판매하거나 브랜드 홍보 미션을 수행할 수 있으며, 정산은 성과 기반으로 이루어집니다.

| 모델 | 전체 이름 | 의미 |
|------|-----------|------|
| **CPS** | Cost Per Sale | 판매 금액 기준 정산 |
| **CPE** | Cost Per Engagement | 반응/참여 기준 정산 |
| **CPM** | Cost Per Mille | 조회수 기준 정산 |

<img src="presentation/monetize-cn.png" width="30%">

---

### 📢 Publish — 콘텐츠 발행 에이전트

전 세계 10개 이상의 주요 플랫폼에 콘텐츠를 한 번에 배포할 수 있어, 플랫폼별 수동 업로드 부담을 줄여줍니다.

- **멀티채널 배포**: Douyin, Kuaishou, Bilibili, Rednote, TikTok, YouTube, Facebook, Instagram, Threads, X(Twitter), Pinterest, LinkedIn 지원
- **캘린더 스케줄링**: 여러 플랫폼의 게시 일정을 한 번에 계획 가능

<img src="presentation/publish-cn.png" width="30%"> <img src="presentation/channel-cn.png" width="30%">

> ▶ 데모 영상 보기

<a href="https://www.youtube.com/watch?v=5041jEKaiU8">
  <img src="https://img.youtube.com/vi/5041jEKaiU8/0.jpg" alt="Publish Demo Video" width="480">
</a>

---

### 💬 Engage — 콘텐츠 상호작용 에이전트

AiToEarn 브라우저 확장 프로그램을 통해 지원되는 플랫폼 전반에서 상호작용 운영을 자동화합니다.

- **자동 액션**: 좋아요, 저장, 팔로우 등을 대량 자동화
- **AI 댓글 응답**: 각 댓글에 맞는 응답을 LLM으로 생성
- **댓글 신호 탐지**: “링크 주세요”, “어디서 사요?” 같은 전환 신호를 빠르게 포착
- **브랜드 모니터링**: 브랜드 언급을 실시간 추적하고 이슈에 참여

> ▶ 데모 영상 보기

<a href="https://youtu.be/-QoHNrZBmp0">
  <img src="./presentation/engage-thumbnail-cn.png" alt="Engage Demo Video" width="480">
</a>

---

### 🎨 Create — 콘텐츠 제작 에이전트

에이전트 방식으로 콘텐츠 제작 워크플로를 재구성했습니다. 필요한 콘텐츠만 설명하면, 아이디어부터 완성본까지 자동으로 처리합니다.

**영상 콘텐츠**: Grok, Veo, Seedance 같은 영상 생성 모델과 번역/편집 모듈을 호출해 영상 제작을 자동화합니다.

**이미지/텍스트 콘텐츠**: Nano Banana 같은 상위 이미지 모델을 활용해 고품질 비주얼 콘텐츠를 자동 생성합니다.

**대량 생성**: 여러 작업을 한 번에 넣어 에이전트가 병렬로 콘텐츠를 생산할 수 있어, 대량 배포나 매트릭스 계정 운영에 적합합니다.

> ▶ 데모 영상 보기

<a href="https://youtu.be/y900LxIrZT4">
  <img src="./presentation/display-1.5.2png.png" alt="Create Demo Video" width="480">
</a>

---

<h2 id="use-web">① 웹사이트에서 바로 사용</h2>

가장 간단한 방법입니다. 브라우저만 열면 바로 사용할 수 있습니다.

- 🇨🇳 중국 사용자: **[aitoearn.cn](https://aitoearn.cn/)**
- 🌍 글로벌 사용자: **[aitoearn.ai](https://aitoearn.ai/)**

---

<h2 id="get-api-key">🔑 API Key 받는 방법</h2>

> 방법 ②③④에는 모두 API Key가 필요합니다. 한 번만 발급받으면 공통으로 사용할 수 있습니다.

**3단계**:

1. [aitoearn.cn](https://aitoearn.cn/) 또는 [aitoearn.ai](https://aitoearn.ai/)에 접속해 회원가입/로그인
2. 왼쪽 메뉴의 **Settings** 클릭
3. **API Key**에서 Create를 눌러 생성 후 복사

<img src="presentation/app-screenshot/0.%20api-key/api-key-settings.png" alt="Get API Key" width="600">

> ⚠️ API Key는 안전하게 보관하고, 타인과 공유하지 마세요.

---

<h2 id="use-in-openclaw">② OpenClaw에서 사용</h2>

> 전제 조건: [API Key 발급 완료](#get-api-key)

**플러그인 설치**

```bash
npx -y @aitoearn/openclaw-plugin-cli
```

처음 실행하면 안내에 따라 필요한 항목을 선택하고 API Key를 입력해 설정을 완료하세요.

설치 후에는 OpenClaw 안에서 AiToEarn 수익화 작업을 직접 받아 실행할 수 있습니다.

<img src="presentation/openclaw-earn-demo.png" alt="Run AiToEarn earning tasks in OpenClaw" width="360">

---

<h2 id="use-in-claude">③ Claude / Cursor / 기타 AI 도구에서 사용</h2>

> 전제 조건: [API Key 발급 완료](#get-api-key)

AiToEarn는 MCP를 지원하는 모든 AI 어시스턴트와 연동할 수 있습니다.

<details open>
<summary><b>Claude Desktop</b></summary>

`claude_desktop_config.json`에 아래를 추가하세요:

```json
{
  "mcpServers": {
    "aitoearn": {
      "type": "http",
      "url": "https://aitoearn.ai/api/unified/mcp",
      "headers": {
        "x-api-key": "your-api-key"
      }
    }
  }
}
```

</details>

<details>
<summary><b>Cursor</b></summary>

Cursor의 MCP 설정에 아래를 추가하세요:

```
MCP URL: https://aitoearn.ai/api/unified/mcp
Auth Header: x-api-key: your-api-key
```

</details>

<details>
<summary><b>기타 AI 도구 (공통 설정)</b></summary>

MCP 호환 도구라면 아래 두 값만 필요합니다.

| 설정 항목 | 값 |
|-----------|----|
| **MCP URL** | `https://aitoearn.ai/api/unified/mcp` |
| **Auth Header** | `x-api-key: your-api-key` |

SSE 방식도 지원합니다: `https://aitoearn.ai/api/unified/sse`

</details>

> 💡 셀프호스팅 환경이라면 `aitoearn.ai` 대신 자신의 주소(예: `localhost:8080`)로 바꾸면 됩니다.

---

<h2 id="use-docker">④ Docker 원클릭 배포</h2>

> 전제 조건: [Docker](https://docs.docker.com/get-docker/) 설치 완료

자체 서버에서 AiToEarn를 운영하려는 팀을 위한 방식입니다. DB를 수동으로 설치할 필요 없이 3개 명령으로 시작할 수 있습니다.

```bash
git clone https://github.com/yikart/AiToEarn.git
cd AiToEarn
docker compose up -d
```

시작 후 **[http://localhost:8080](http://localhost:8080)** 에 접속하면 됩니다.

#### Relay 설정 (강력 권장)

> **왜 Relay가 필요한가요?** 소셜 계정으로 콘텐츠를 발행하려면 OAuth 개발자 자격이 필요한데, Relay를 쓰면 공식 aitoearn.ai 쪽 자격을 재활용할 수 있어 각 플랫폼마다 개발자 계정을 따로 만들 필요가 없습니다.

`docker-compose.yml`의 `aitoearn-server`에 아래를 추가하세요:

```yaml
RELAY_SERVER_URL: https://aitoearn.ai/api
RELAY_API_KEY: your-api-key
RELAY_CALLBACK_URL: http://127.0.0.1:8080/api/plat/relay-callback
```

그 다음 재시작:

```bash
docker compose restart aitoearn-server
```

> 📖 프로덕션 설정, AI 서비스, OAuth, 스토리지까지 포함한 전체 배포 가이드는 [DOCKER_DEPLOYMENT_EN.md](DOCKER_DEPLOYMENT_EN.md)를 참고하세요.

---

<h2 id="use-source">⑤ 소스코드로 개발</h2>

<details>
<summary>🧪 백엔드와 프론트엔드를 수동으로 실행 (개발 모드)</summary>

로컬 개발/디버깅용입니다. MongoDB/Redis는 Docker로 띄우거나, 직접 운영 중인 서비스로 연결해도 됩니다.

#### 1. 백엔드 실행

```bash
cd project/aitoearn-backend
pnpm install
# 로컬 개발용 설정 파일 복사
cp apps/aitoearn-ai/config/config.js apps/aitoearn-ai/config/local.config.js
cp apps/aitoearn-server/config/config.js apps/aitoearn-server/config/local.config.js
pnpm nx serve aitoearn-ai
# 다른 터미널에서
pnpm nx serve aitoearn-server
```

#### 2. 프론트엔드 `aitoearn-web` 실행

```bash
pnpm install
pnpm run dev
```

</details>

<details>
<summary>🖥️ Electron 데스크톱 프로젝트 실행</summary>

```bash
# 저장소 클론
git clone https://github.com/yikart/AttAiToEarn.git

# 디렉터리 이동
cd AttAiToEarn

# 의존성 설치
npm install

# sqlite 컴파일 (better-sqlite3는 node-gyp와 로컬 Python 필요)
npm run rebuild

# 개발 실행
npm run dev
```

Electron 프로젝트는 AiToEarn 데스크톱 클라이언트를 제공합니다.

</details>

## 기여 가이드

참여를 원하시면 [Contributing Guide](./CONTRIBUTING.md)를 참고하세요.

## 문의

사용 중 어려움, 질문, 예상치 못한 동작이 있다면 먼저 [GitHub Issues](https://github.com/yikart/AiToEarn/issues)에 남겨 주세요.

- Telegram: [https://t.me/harryyyy2025](https://t.me/harryyyy2025)
- WeChat: QR 코드 스캔

<img src="presentation/wechat.jpg" alt="WeChat QR Code" width="200">

## 추천

- [MuseTalk](https://github.com/TMElyralab/MuseTalk)
- [video_spider](https://github.com/5ime/video_spider)
- [CosyVoice](https://github.com/FunAudioLLM/CosyVoice?tab=readme-ov-file)
- [facefusion](https://github.com/facefusion/facefusion)
- [NarratoAI](https://github.com/linyqh/NarratoAI)
- [MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo)
