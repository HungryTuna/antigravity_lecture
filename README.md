# 안티그래비티(Antigravity) 초보자 교육자료 웹 앱

Google Antigravity, Skills, MCP(Stitch), Gemini API를 비개발자도 쉽게 이해하고 실습할 수 있도록 제작된 반응형 웹 교육 가이드 및 데모 웹 애플리케이션입니다.

🌐 **배포 사이트(GitHub Pages)**: [https://hungrytuna.github.io/antigravity_lecture/](https://hungrytuna.github.io/antigravity_lecture/)

---

## 📌 주요 기능 및 특징

1. **상세한 커리큘럼 및 가이드**:
   - **01장**: 안티그래비티 개념, 에이전트 vs 챗봇 비교, GEMINI.md, Skill
   - **02장**: 설치 및 초기 설정
   - **03장**: Skill.sh 스킬 설정 (전역/지역)
   - **04장**: Stitch MCP 도구 연동
   - **05장**: Gemini API 키 발급 및 보안 수칙
   - **06장**: 기도문 자동 생성기 실습 프롬프트 (STEP 1 ~ STEP 9)
2. **인프레임(In-frame) 동영상 재생**:
   - 메인 히어로 섹션의 표지 이미지(`image1.png`) 및 재생 버튼을 클릭하면 팝업 창 없이 해당 이미지 프레임 안에서 즉시 안티그래비티 소개 영상이 부드럽게 인라인으로 재생됩니다.
   - 브라우저 표준 컨트롤러(일시정지, 음량, 타임바, 전체화면)를 통해 프레임 내에서 편리하게 시청할 수 있습니다.
3. **사용자 인터랙션 및 편의 기능**:
   - 프롬프트 원클릭 복사(Copy) 기능
   - 목차 스크롤 스파이(Scroll Spy)
   - 모바일/태블릿 반응형 내비게이션 지원

---

## 💻 설치 및 사전 요구 사항

외부 빌드 도구나 복잡한 종속성 없이, 순수 웹 표준(HTML5, CSS3, Vanilla JavaScript)으로 구현되어 있습니다.

- 웹 브라우저 (Google Chrome, Microsoft Edge 등 최신 브라우저 권장)
- 로컬 웹 서버 실행 환경 (Python 3 또는 Node.js)

---

## 🚀 실행 방법

### 방법 1. 배포된 온라인 사이트 바로가기 (별도 설치 불필요)
브라우저에서 아래 URL로 접속하시면 즉시 웹 앱을 이용할 수 있습니다:
- [https://hungrytuna.github.io/antigravity_lecture/](https://hungrytuna.github.io/antigravity_lecture/)

---

### 방법 2. Python 로컬 웹 서버 사용 (권장)

1. 터미널을 열고 `web` 디렉토리로 이동합니다:
   ```bash
   cd web
   ```

2. 파이썬 기본 HTTP 서버를 실행합니다:
   ```bash
   python -m http.server 8080
   ```

3. 브라우저에서 아래 주소로 접속합니다:
   ```
   http://localhost:8080
   ```

---

### 방법 3. Node.js (npx serve) 사용

1. 터미널에서 `web` 디렉토리로 이동합니다:
   ```bash
   cd web
   ```

2. npx serve 명령어로 로컬 서버를 구동합니다:
   ```bash
   npx serve .
   ```

3. 터미널에 표시되는 주소(예: `http://localhost:3000`)로 접속합니다.

---

## 📂 프로젝트 구조

```text
├── .github/
│   └── workflows/
│       └── deploy.yml       # GitHub Pages 자동 배포 워크플로우
├── web/
│   ├── index.html           # 메인 교육자료 단일 페이지 웹 애플리케이션
│   └── assets/              # 가이드 이미지 및 인프레임 시연 동영상
├── .gitignore               # 불필요한 파일 제외 설정
├── design_guide.md          # 디자인 시스템 및 테마 가이드
└── README.md                # 프로젝트 안내 문서
```
