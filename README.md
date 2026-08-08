# 성희윤 | Frontend Engineer

> 요구사항 변화에 강한 구조를 설계하고, 측정 가능한 결과로 검증합니다.

기능 추가가 반복될수록 커지는 변경 비용을 줄이는 구조를 설계합니다.
Next.js 기반 에디터·렌더러와 위치 기반 서비스를 1인 개발하며 확장성·성능·상태 설계를 테스트와 지표로 검증해왔습니다.

## Selected Projects

### Layer0 Studio

**No-code Website Builder SaaS**

템플릿을 선택해 콘텐츠를 편집하고, 단일 페이지 또는 멀티페이지 웹사이트를 공개할 수 있는 서비스입니다.

- 신규 템플릿 추가 시 편집기 공통 코드 수정 **0줄**
- Lighthouse Mobile **55 → 90**
- 랜딩 초기 CSS **11개 → 1개**

[Live](https://layer0-studio.vercel.app) · [Repository](https://github.com/sungheeyoon/layer0-studio)

`Next.js` `React` `TypeScript` `Supabase` `Vitest` `Vercel`

### 동네속닥

**Location-based Community Service**

지도에서 주변의 생활 이슈를 확인하고 제보·투표·댓글로 공유하는 서비스입니다.

- 통제된 부하 테스트에서 API p50 **8.7초 → 0.43초**
- 처리량 **2.27 → 28.70 RPS (12.6배)**
- 지도 SDK 이벤트와 제품의 조회 기준을 분리해 불필요한 상태 확정 방지

[Live](https://dongne-sokdak.vercel.app) · [Repository](https://github.com/sungheeyoon/dongne-sokdak)

`Next.js` `React` `TypeScript` `FastAPI` `PostgreSQL/PostGIS` `Kakao Maps` `TanStack Query`

> 동네속닥 성능 수치는 로컬 단일 프로세스·공유 Supabase·합성 데이터 환경에서 비교군별 3회 측정한 중앙값이며 운영 SLA가 아닙니다.

## Tech

- **Frontend** — Next.js · React · TypeScript · TanStack Query
- **Backend** — FastAPI · PostgreSQL · Supabase
- **Architecture** — Clean Architecture · 의존성·상태 경계 설계 · Optimistic Concurrency Control
- **Tools** — Git · GitHub · Vercel · Vitest

## Links

- [Portfolio](https://cautious-jester-d10.notion.site/Frontend-Engineer-397bb16c585d80c1ba36c80797f927ca)
- [Email](mailto:torushy@gmail.com)
