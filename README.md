# kt cloud TECH UP 1기 현장 스케치

![kt cloud TECH UP](https://www.genspark.ai/api/files/s/JicupQXg)

> 클라우드 전문가를 향한 첫 걸음, kt cloud TECH UP 1기의 생생한 현장을 담았습니다.

## 🚀 프로젝트 소개

kt cloud TECH UP 1기 현장 스케치 웹사이트는 교육생들의 활동과 성장 과정을 시각적으로 보여주는 정적 웹사이트입니다.

### 주요 기능
- 🎨 **인터랙티브 우주 테마**: 떠다니는 행성과 별들이 있는 히어로 섹션
- 📸 **현장 스케치 갤러리**: 9개의 현장 사진을 좌우로 넘기며 확인
- 💼 **프로그램 소개**: 이론/프로젝트 현장과 해커톤 현장 소개
- 💬 **수료생 후기**: 1기 교육생들의 생생한 경험담
- 📱 **완전 반응형**: 데스크탑, 태블릿, 모바일 모두 지원

## 📂 프로젝트 구조

```
kt-techup-showcase/
├── index.html          # 메인 HTML 파일
├── README.md           # 프로젝트 설명서
├── IMAGE_GUIDE.md      # 이미지 추가 가이드
└── .gitignore          # Git 제외 파일 목록
```

## 🛠️ 기술 스택

- **HTML5**: 시맨틱 마크업
- **CSS3**: 애니메이션 및 반응형 디자인
- **JavaScript (Vanilla)**: 갤러리 슬라이더, 스크롤 애니메이션
- **Google Fonts**: Noto Sans KR

## 🎯 주요 섹션

### 1. 히어로 섹션
- kt cloud 로고
- 우주 배경 + 떠다니는 행성 애니메이션
- "1기 현장 스케치" 타이틀

### 2. 현장 스케치 갤러리
- 9개의 현장 사진
- 좌우 화살표 네비게이션
- 하단 인디케이터로 직접 이동
- 2:1 비율, 1360px 최대 넓이

### 3. 이론/프로젝트 현장 (3개 카드)
- kt cloud 현직자 멘토링
- kt cloud 현직자 특강
- 팀 프로젝트

### 4. 해커톤 현장 (4개 카드)
- TECH UP 연합 해커톤
- 팀 협업 & 아이디어 구현
- 최종 발표 & 시연
- 시상 & 네트워킹

### 5. 수료생 후기 (4개 카드)
- 교육생들의 생생한 후기
- 프로필 + 후기 내용 + 태그

### 6. CTA 섹션
- 2기 모집 안내

## 🚀 시작하기

### 1. 저장소 클론

```bash
git clone https://github.com/your-username/kt-techup-showcase.git
cd kt-techup-showcase
```

### 2. 로컬에서 실행

간단히 `index.html` 파일을 브라우저에서 열면 됩니다.

```bash
# macOS
open index.html

# Windows
start index.html

# Linux
xdg-open index.html
```

또는 Live Server를 사용하여 실행:

```bash
# VS Code의 Live Server 확장 프로그램 사용
# 또는 Python 내장 서버
python -m http.server 8000

# Node.js http-server
npx http-server
```

## 🎨 브랜드 컬러

- **Primary Red**: `#E63312` (kt cloud 브랜드 컬러)
- **Dark Navy**: `#1a1a2e`, `#16213e`
- **Pure Black**: `#0a0a0a`
- **White**: `#ffffff`

## 📱 반응형 브레이크포인트

```css
/* Mobile */
@media (max-width: 767px) { ... }

/* Tablet */
@media (max-width: 1024px) { ... }

/* Desktop */
@media (min-width: 1025px) { ... }
```

## 🌐 배포

### GitHub Pages

1. GitHub 저장소 설정 → Pages
2. Source를 `main` 브랜치로 선택
3. 자동으로 배포됨

### Netlify

1. [Netlify](https://netlify.com)에 로그인
2. "New site from Git" 클릭
3. GitHub 저장소 연결
4. 자동 배포

### Vercel

1. [Vercel](https://vercel.com)에 로그인
2. "New Project" 클릭
3. GitHub 저장소 가져오기
4. 자동 배포

## 🖼️ 이미지 커스터마이징

더 자세한 이미지 추가 방법은 [IMAGE_GUIDE.md](./IMAGE_GUIDE.md)를 참조하세요.

### 빠른 가이드

1. **갤러리 이미지**: `index.html`에서 `.gallery-item-slide` 내부의 이미지 URL 수정
2. **프로그램 카드 이미지**: `.career-card-image` 내부의 플레이스홀더를 실제 이미지로 교체
3. **권장 이미지 사양**:
   - 갤러리: 2:1 비율 (예: 1360x680px)
   - 카드 이미지: 16:9 비율 (예: 640x360px)
   - 포맷: JPG, PNG, WebP

## 📝 텍스트 커스터마이징

### 타이틀 변경

```html
<!-- index.html 라인 751 -->
<div class="hero-title-text">
    1기 현장 스케치  <!-- 여기를 수정 -->
</div>
```

### 프로그램 설명 변경

```html
<!-- 각 카드의 career-card-description 부분 수정 -->
<p class="career-card-description">
    여기에 프로그램 설명을 입력하세요
</p>
```

## 🐛 문제 해결

### 이미지가 표시되지 않을 때
- 이미지 URL이 유효한지 확인
- 브라우저 콘솔에서 에러 확인
- CORS 문제인 경우 이미지를 로컬에 저장

### 갤러리가 작동하지 않을 때
- JavaScript 콘솔 에러 확인
- 브라우저 호환성 확인 (Chrome 90+, Firefox 88+, Safari 14+)

## 🤝 기여하기

이 프로젝트는 kt cloud TECH UP 1기 현장 스케치를 위한 것입니다. 개선 사항이나 버그를 발견하시면 이슈를 등록해 주세요.

## 📄 라이선스

이 프로젝트는 교육 목적으로 제작되었습니다.

## 📞 문의

kt cloud TECH UP 관련 문의: [kt cloud 공식 웹사이트](https://cloud.kt.com)

---

**Made with ❤️ by kt cloud TECH UP 1기**
