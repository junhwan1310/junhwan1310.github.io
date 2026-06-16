# 박준환 Portfolio OS

정적 HTML/CSS/JavaScript 기반 포트폴리오입니다.  
운영체제형 데스크톱 UI 안에서 ERP, 모바일 앱, 수강 신청 폼, 정책 매칭, SQL 학습 앱을 확인할 수 있습니다.

## 실행 방법

1. 저장소를 내려받거나 ZIP을 압축 해제합니다.
2. 루트의 `index.html` 파일을 브라우저에서 엽니다.
3. 바탕화면 아이콘을 더블클릭하면 각 프로젝트 창이 열립니다.

## 포함 프로젝트

### ERP Project

ERP 업무 화면을 기능 항목별 탭으로 나누어 정리했습니다.

- 대시보드/매출
- 상품 관리
- 고객 관리
- 생산/재고
- 거래처/인사
- 엑셀/문서 출력
- ERP 화면 GIF 22개 포함

### App Project

반려동물 관리 앱 화면을 GIF로 확인할 수 있는 프로젝트입니다.

### LiveClass Enrollment Form

React + TypeScript 기반 다단계 수강 신청 폼입니다.

- 강의 선택 및 카테고리 필터
- 개인/단체 신청 조건부 입력
- Zod 기반 유효성 검증
- Mock API 기반 제출 흐름
- localStorage 기반 임시 저장
- Vitest 테스트 코드 포함

실행용 정적 HTML은 `apps/liveclass_enrollment/index.html`에 있고, 원본 소스는 `source/liveclass-fe-a-enrollment-form/`에 있습니다.

### Policy Matcher

정적 정책 데이터를 조건에 따라 필터링하고 추천 결과를 보여주는 정책 매칭 데모입니다.

### SQL SELECT Study App

SQL SELECT 문제와 예시 쿼리를 확인할 수 있는 학습용 HTML 앱입니다.

## 폴더 구조

```txt
.
├── index.html
├── apps/
│   ├── liveclass_enrollment/
│   ├── policy_matcher_v10_with_easy_header.html
│   └── sql_select_study_app.html
├── assets/
│   ├── app_screen_1.gif
│   ├── app_screen_2.gif
│   └── erp/
└── source/
    └── liveclass-fe-a-enrollment-form/
```

## GitHub Pages 배포

정적 사이트이므로 별도 빌드 없이 GitHub Pages에서 루트(`/`)를 배포 소스로 지정하면 됩니다.  
배포 기준 파일은 루트의 `index.html`입니다.

## LiveClass 원본 소스 실행

LiveClass 프로젝트를 개발 환경에서 다시 실행하려면 다음 명령어를 사용합니다.

```bash
cd source/liveclass-fe-a-enrollment-form
npm install
npm run dev
```

테스트 실행:

```bash
npm test
```

## 정리 기준

- `.git`, `node_modules`, `dist`, `.env` 파일은 포함하지 않았습니다.
- 외부 API 키나 민감정보는 포함하지 않았습니다.
- 포트폴리오 제출 및 GitHub Pages 배포를 기준으로 정리했습니다.
