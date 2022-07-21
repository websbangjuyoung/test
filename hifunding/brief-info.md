## 폴더구조
- src: 소스파일 폴더 (파일 형태에 따라 분류)
    - assets: 이미지 등 에셋 파일
    - components: react component 
        - common: 범용 컴포넌트
        - layout: 레이아웃 컴포넌트
        - form: 폼 관련 컴포넌트
        - 그 외 목적에 따라 폴더 분류
    - constants: 상수 정의
    - hooks: custom hooks 관련 코드
    - libs: 외부 유틸 라이브러리 정의
    - pages: 웹 페이지
    - services: 하이펀딩 API 서비스
    - store: recoil state 전역 상태 정의
    - styles: 테마 등 범용 스타일 정의
    - types: 타입 정의
    - utils: 범용 헬퍼 함수 정의
    - App.tsx: 리액트 최상위 컴포넌트 (예: 페이지 별로 라우트 정의)
    - index.tsx: 리액트 진입 컴포넌트 (예: mui / react-query / react-router-dom  등 전역으로 적용)
- .env: 환경 설정 파일 (ex: API endpoint 정의)
- .eslintrc.js: 스크립트 기본 문법 검사 규칙 정의
- .prettierrc: 코딩 스타일 정의
- package.json: 프로젝트 정보 및 패키지 의존성 관리 명세
- tsconfig.json: 타입 스크립트 설정
- yarn.lock: 패키지 잠금 파일 (현재 사용하고 있는 패키지들의 정확한 버젼 정보 명시)

## node 및 패키지
### node
`node` v16 `LTS`(gallium) 버젼 사용
### 패키지 매니저
`yarn` 1.22

### 주요 패키지
- react / react-dom: 리액트 라이브러리
- typescript: 타입스크립트
- @mui: 리액트 기반 UI 라이브러리
- axios: Promise 기반 HTTP 클라이언트 라이브러리
- react-query: 데이터 페칭 / 캐싱 등을 효율적으로 처리할 수 있게 도와주는 라이브러리
- dayjs: 날짜 포맷터
- react-daum-postcode: 다음 주소 검색
- react-hook-form: 폼처리
- yup: 폼 유효성 검사
- react-icons: 아이콘 
- react-imask: 값 마스킹 처리 (예: 금액일 경우 천단위로 콤마 표시)
- react-router / react-router-dom: 라우터 처리
- recharts: 차트
- recoil: 전역 상태 관리 (예: 회원 인증 토큰 관리)

## 프로젝트 실행

### 최초 실행시
````
yarn // 의존성 패키지 설치 (yarn.lock 파일에 명시된 버젼으로 설치됨)
````

### 개발 모드로 실행
````
yarn start
````

### 배포 모드로 실행
````
yarn build 
````


