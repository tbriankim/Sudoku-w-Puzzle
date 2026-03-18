# 두뇌 개발 스도쿠 🧩

동물 퍼즐을 수집하는 스도쿠 게임. React + Vite 단일 파일 구조.

---

## 로컬 실행

```bash
npm install
npm run dev
```
브라우저에서 `http://localhost:5173` 열기

---

## GitHub + Vercel 배포 (모바일 링크)

### 1단계 — GitHub에 올리기

1. [github.com](https://github.com) → 로그인 (없으면 무료 가입)
2. 우측 상단 `+` → **New repository**
3. Repository name: `sudoku-game` → **Create repository**
4. 화면에 나오는 명령어 대신 아래 방법 사용:
   - **Upload files** 클릭
   - 이 폴더의 모든 파일을 드래그하여 업로드
   - `node_modules` 폴더는 업로드 **하지 말 것**
5. **Commit changes** 클릭

### 2단계 — Vercel로 배포

1. [vercel.com](https://vercel.com) → **Sign up with GitHub**
2. **Add New Project** → GitHub repository 선택
3. Framework: **Vite** 자동 감지됨
4. **Deploy** 클릭
5. 배포 완료 후 링크 받기: `https://sudoku-game-xxx.vercel.app`

### 3단계 — 모바일 홈화면에 추가

**iPhone:**
Safari에서 링크 열기 → 하단 공유 버튼 → **홈 화면에 추가**

**Android:**
Chrome에서 링크 열기 → 우측 상단 메뉴 → **홈 화면에 추가**

---

## 파일 구조

```
sudoku-game/
├── src/
│   ├── App.jsx        ← 게임 전체 코드 (여기만 수정)
│   └── index.jsx      ← React 진입점
├── index.html         ← HTML 템플릿
├── package.json       ← 의존성
├── vite.config.js     ← 빌드 설정
└── .gitignore
```

## 게임 수정하기

`src/App.jsx` 파일만 수정하면 됩니다.
섹션 구조 (Ctrl+F로 검색):

- `§ 1` 스도쿠 엔진
- `§ 2` 음악 엔진  
- `§ 3` 레벨/테마 상수 ← 난이도 조정
- `§ 4` 동물 그림 ← 동물 추가/수정
- `§ 5` 상태/리듀서
- `§ 6` 퍼즐 그리드
- `§ 7` 스도쿠 보드
- `§ 8` 모달
- `§ 9` 화면들
- `§10` 앱 루트
