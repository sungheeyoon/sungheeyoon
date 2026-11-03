# 성희윤 · 프론트엔드 개발자

서비스를 처음부터 운영까지 혼자 만들어 왔습니다. Next.js와 TypeScript로 화면을 만들고, 필요하면 API와 데이터베이스도 직접 설계합니다.
최근에는 구현을 AI 코딩 에이전트에게 맡기고, 저는 무엇을 만들지 정하고 그 결과를 테스트와 기록으로 검증합니다.

## 프로젝트

### [만날지도](https://github.com/sungheeyoon/saju) — 사주·궁합·인연 서비스

생년월일시로 사주를 계산하고, 그 근거 위에서 AI가 풀이를 쓰는 서비스입니다. 웹과 iOS·Android 앱, 2026.08 – 현재(운영 베타).

- 만세력 엔진을 순수 TypeScript로 분리하고, 학파마다 갈리는 규칙을 옵션으로 둔 뒤 적용한 보정 내역을 결과와 함께 반환
- AI가 쓴 풀이는 저장 전에 검사: 출생 정보 유출·근거 없는 판정·그릴 수 없는 형식은 막고, 품질 문제는 기록
- 에이전트 작업 규칙: 결정은 ADR(220건)로 남기고, 권한을 되돌릴 수 있는가로 나눠 배포는 사람이 승인. PR 826건을 테스트·CI를 거쳐 머지

[mannalmap.com](https://mannalmap.com) · `Next.js` `React` `TypeScript` `Supabase` `Expo` `Vercel` `OpenAI`

### [Layer0 Studio](https://github.com/sungheeyoon/layer0-studio) — 노코드 웹사이트 빌더

템플릿을 골라 코딩 없이 웹사이트를 만들고 게시하는 서비스입니다. 2026.03 – 현재.

- 편집 필드 스키마 하나로 UI와 렌더러를 묶어, 새 템플릿을 추가해도 편집기 공통 코드 변경 0줄
- 자동 저장을 걷어내고 작업본과 공개본을 분리해 게시 전 편집이 공개 페이지에 나가지 않게 함
- 초기 로딩 경로에서 안 쓰는 의존성을 빼서 Lighthouse Mobile 72 → 97, LCP 13.1초 → 2.6초

[layer0-studio.vercel.app](https://layer0-studio.vercel.app) · `Next.js` `React` `TypeScript` `Supabase` `Vitest`

### [동네속닥](https://github.com/sungheeyoon/dongne-sokdak) — 지도 기반 동네 이슈 커뮤니티

지도에서 주변 생활 이슈를 보고 제보·투표·댓글로 나누는 서비스입니다. 2025.07 첫 공개.

- SQL과 API를 따로 측정해 동기 Supabase 호출의 이벤트 루프 점유를 찾아냄: API p50 8.7초 → 0.43초, 처리량 2.27 → 28.70 RPS
- 지도 SDK 이벤트와 조회 기준을 나눠, 드래그·확대 20회에도 조회 기준 변경 0회

[dongne-sokdak.vercel.app](https://dongne-sokdak.vercel.app) · `Next.js` `FastAPI` `PostgreSQL/PostGIS` `Kakao Maps`

<sub>동네속닥 수치는 로컬 단일 프로세스 · 합성 데이터 · 3회 중앙값이며 운영 SLA가 아닙니다. Layer0 수치는 2026.08 프로덕션 배포 재측정(Lighthouse Mobile 3회 중앙값)입니다.</sub>

## 기술

- **Frontend** Next.js · React · TypeScript · TanStack Query · Tailwind CSS
- **Mobile** Expo · React Native
- **Backend · DB** Supabase(PostgreSQL) · PostGIS · FastAPI
- **Test · 측정** Vitest · Playwright · pgTAP · Lighthouse · Locust

## 연락

torushy@gmail.com
