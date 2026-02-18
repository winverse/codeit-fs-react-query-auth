# React Query Auth Frontend

App Router 기반 Next.js 16 프로젝트입니다.

## 실행 방법

1. 의존성 설치

```bash
pnpm install
```

2. 환경 변수 파일 생성

```bash
cp .env.example .env.local
```

3. 개발 서버 실행

```bash
pnpm dev
```

기본 URL: `http://localhost:3000`

## 백엔드 연결

- 백엔드 기본 URL: `http://localhost:5001` (`/api`는 내부에서 자동으로 붙음)
- 브라우저에서 백엔드를 직접 호출하므로 백엔드에서 CORS(`origin`, `credentials`)를 설정해야 합니다.

## 주요 기능

- React Query `useMutation`: 회원가입/로그인 요청
- React Query `useQuery`: 사용자 목록 조회
- 회원가입 성공 후 사용자 목록 재조회(invalidate)로 생성 여부 확인
