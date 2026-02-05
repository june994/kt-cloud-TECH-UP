# 이미지 추가 가이드 📸

kt cloud TECH UP 웹사이트에 실제 현장 사진을 추가하는 상세 가이드입니다.

## 📋 필요한 이미지 목록

### 🎯 우선순위 높음

#### 1. 현장 스케치 갤러리 (6장) - **필수**
| 번호 | 파일명 | 설명 | 권장 크기 | 비율 |
|------|--------|------|-----------|------|
| 1 | `hackathon.jpg` | 해커톤 현장 - 팀원들이 협업하는 모습 | 1920x1080px | 16:9 |
| 2 | `mentoring.jpg` | 멘토링 - 현직자와 대화하는 장면 | 1920x1080px | 16:9 |
| 3 | `lecture.jpg` | 특강 - 강연 듣는 수강생들 | 1920x1080px | 16:9 |
| 4 | `codereview.jpg` | 코드리뷰 - 코드 보며 피드백 받는 장면 | 1920x1080px | 16:9 |
| 5 | `presentation.jpg` | 발표 - 프로젝트 발표하는 모습 | 1920x1080px | 16:9 |
| 6 | `graduation.jpg` | 수료식 - 단체 사진 또는 수료증 | 1920x1080px | 16:9 |

#### 2. 커리어 카드 이미지 (6장) - **권장**
| 번호 | 파일명 | 설명 | 권장 크기 |
|------|--------|------|-----------|
| 1 | `career-mentoring.jpg` | 멘토링 관련 이미지 | 800x560px |
| 2 | `career-hackathon.jpg` | 해커톤 관련 이미지 | 800x560px |
| 3 | `career-lecture.jpg` | 특강 관련 이미지 | 800x560px |
| 4 | `career-codereview.jpg` | 코드리뷰 관련 이미지 | 800x560px |
| 5 | `career-hiring.jpg` | 채용/커리어 관련 이미지 | 800x560px |
| 6 | `career-consulting.jpg` | 컨설팅 관련 이미지 | 800x560px |

#### 3. 브랜드 이미지 (1장) - **선택**
| 파일명 | 설명 | 권장 크기 |
|--------|------|-----------|
| `kt-cloud-logo.png` | kt cloud 로고 (투명 배경) | 400x160px |

---

## 🛠️ 이미지 추가 방법

### 방법 1: 갤러리 이미지 추가 (현장 스케치)

#### Step 1: 이미지 파일 준비
```
프로젝트 폴더/
├── index.html
├── images/              ← 이 폴더 생성
│   ├── hackathon.jpg
│   ├── mentoring.jpg
│   ├── lecture.jpg
│   ├── codereview.jpg
│   ├── presentation.jpg
│   └── graduation.jpg
```

#### Step 2: HTML 코드 수정

**해커톤 이미지 (1번)**

찾기:
```html
<div class="gallery-item animate-on-scroll">
    <div class="gallery-placeholder">
        <div class="gallery-placeholder-icon">🔥</div>
        <div class="gallery-placeholder-text">해커톤 현장 이미지</div>
    </div>
    <div class="gallery-caption">
        <h3>연합 해커톤 현장</h3>
        <p>팀별 프로젝트를 완성하며 실전 경험 쌓기</p>
    </div>
</div>
```

교체:
```html
<div class="gallery-item animate-on-scroll">
    <img src="images/hackathon.jpg" alt="연합 해커톤 현장" style="width: 100%; height: 100%; object-fit: cover; border-radius: 20px;">
    <div class="gallery-caption">
        <h3>연합 해커톤 현장</h3>
        <p>팀별 프로젝트를 완성하며 실전 경험 쌓기</p>
    </div>
</div>
```

**나머지 5개 이미지도 동일한 방식으로 수정**:
- `mentoring.jpg` → 멘토링 섹션
- `lecture.jpg` → 특강 섹션
- `codereview.jpg` → 코드리뷰 섹션
- `presentation.jpg` → 발표 섹션
- `graduation.jpg` → 수료식 섹션

---

### 방법 2: 커리어 카드 이미지 추가

#### Step 1: 이미지 파일 준비
```
프로젝트 폴더/
├── index.html
├── images/
│   ├── career-mentoring.jpg
│   ├── career-hackathon.jpg
│   ├── career-lecture.jpg
│   ├── career-codereview.jpg
│   ├── career-hiring.jpg
│   └── career-consulting.jpg
```

#### Step 2: HTML 코드 수정

**멘토링 카드 (1번)**

찾기:
```html
<div class="career-card-image">
    <div class="career-card-placeholder">
        <div class="career-placeholder-icon">💬</div>
        <div class="career-placeholder-label">멘토링 활동 이미지를 추가해주세요</div>
    </div>
</div>
```

교체:
```html
<div class="career-card-image">
    <img src="images/career-mentoring.jpg" alt="현직자 멘토링" style="width: 100%; height: 100%; object-fit: cover;">
</div>
```

**나머지 5개 카드도 동일한 방식으로 수정**

---

## 🎨 이미지 최적화 팁

### 1. 이미지 크기 최적화

#### 권장 해상도:
- **갤러리 이미지**: 1920x1080px (Full HD)
- **카드 이미지**: 800x560px
- **로고**: 400x160px

#### 파일 크기:
- 갤러리 이미지: 200-500KB 이하
- 카드 이미지: 100-200KB 이하

### 2. 이미지 포맷 선택

| 포맷 | 용도 | 장점 |
|------|------|------|
| **JPG** | 사진 (갤러리, 카드) | 작은 파일 크기 |
| **PNG** | 로고 (투명 배경) | 투명도 지원 |
| **WebP** | 모든 이미지 | 최적의 압축률 |

### 3. 온라인 압축 도구

- [TinyPNG](https://tinypng.com/) - PNG/JPG 무손실 압축
- [Squoosh](https://squoosh.app/) - 구글 제공, WebP 변환
- [ImageOptim](https://imageoptim.com/) - Mac 전용

---

## 🖼️ 이미지 촬영/선택 가이드

### 갤러리 이미지 (현장 스케치)

#### 📸 촬영 팁:
1. **자연스러운 장면**: 연출보다는 실제 활동 중인 모습
2. **밝은 조명**: 실내 조명이 충분한 환경
3. **다양한 각도**: 정면, 측면, 전체 샷 등 다양하게
4. **인물 중심**: 사람들의 표정과 상호작용 강조
5. **공간감**: 전체 공간이 보이는 와이드 샷 활용

#### 🎯 각 장면별 가이드:

**1. 해커톤 (hackathon.jpg)**
- ✅ 노트북 앞에서 코딩하는 모습
- ✅ 팀원들과 토론하는 장면
- ✅ 화이트보드에 아이디어 스케치
- ❌ 지루하거나 정적인 장면

**2. 멘토링 (mentoring.jpg)**
- ✅ 멘토와 멘티가 대화하는 모습
- ✅ 진지하게 설명 듣는 표정
- ✅ 노트북/자료 보며 토론
- ❌ 형식적인 포즈

**3. 특강 (lecture.jpg)**
- ✅ 강사가 발표하는 장면 + 청중
- ✅ 필기하는 수강생들
- ✅ 집중하는 분위기
- ❌ 빈 좌석이 많은 장면

**4. 코드리뷰 (codereview.jpg)**
- ✅ 화면 보며 코드 설명하는 장면
- ✅ 여러 명이 모니터 보는 모습
- ✅ 진지한 피드백 받는 표정
- ❌ 혼자만 있는 장면

**5. 발표 (presentation.jpg)**
- ✅ 발표자와 청중 모두 보이는 구도
- ✅ 발표 화면 + 발표자
- ✅ 자신감 있는 발표 모습
- ❌ 발표자만 클로즈업

**6. 수료식 (graduation.jpg)**
- ✅ 단체 사진 (전체 수료생)
- ✅ 수료증 받는 순간
- ✅ 축하하는 분위기
- ❌ 일부만 있는 사진

---

## 🚨 주의사항

### 저작권 및 초상권
- ✅ 1기 교육생들의 **사진 사용 동의** 필수
- ✅ 교육 현장에서 직접 촬영한 사진 사용
- ❌ 무단으로 다른 행사 사진 사용 금지
- ❌ 저작권 있는 이미지 무단 사용 금지

### 이미지 품질
- ✅ 해상도: 최소 1920x1080px 이상
- ✅ 흐릿하지 않은 선명한 사진
- ✅ 적절한 밝기와 대비
- ❌ 흔들린 사진
- ❌ 너무 어둡거나 과다 노출

---

## 🔄 이미지가 없는 경우 대안

### 임시 이미지 사용

**Unsplash (무료 고품질 이미지)**
```html
<!-- 예시: 코딩 이미지 -->
<img src="https://images.unsplash.com/photo-1522071820081-009f0129c71c?w=1920" alt="팀워크">
```

**추천 검색어**:
- `coding teamwork`
- `tech conference`
- `students learning`
- `presentation meeting`
- `graduation ceremony`

**주의**: 실제 1기 사진으로 교체 필요!

---

## ✅ 이미지 추가 체크리스트

### 갤러리 (6장)
- [ ] 해커톤 현장 이미지
- [ ] 멘토링 현장 이미지
- [ ] 특강 현장 이미지
- [ ] 코드리뷰 현장 이미지
- [ ] 발표 현장 이미지
- [ ] 수료식 이미지

### 커리어 카드 (6장)
- [ ] 멘토링 카드 이미지
- [ ] 해커톤 카드 이미지
- [ ] 특강 카드 이미지
- [ ] 코드리뷰 카드 이미지
- [ ] 채용 우대 카드 이미지
- [ ] 컨설팅 카드 이미지

### 추가 이미지
- [ ] kt cloud 로고 (선택)
- [ ] OG 이미지 (SNS 공유용, 선택)

---

## 🎬 이미지 추가 후 테스트

### 1. 로컬 테스트
```bash
# 브라우저에서 index.html 열기
# 모든 이미지가 정상적으로 보이는지 확인
```

### 2. 체크 항목
- [ ] 이미지가 깨지지 않고 정상 표시
- [ ] 이미지 비율이 올바름 (찌그러지지 않음)
- [ ] 호버 효과 정상 작동
- [ ] 모바일에서도 정상 표시
- [ ] 로딩 속도가 느리지 않음 (3초 이내)

### 3. 최적화 확인
- [ ] 파일 크기 적절 (500KB 이하)
- [ ] 해상도 적절 (너무 크지 않음)
- [ ] 포맷 적절 (JPG/PNG/WebP)

---

## 💡 FAQ

### Q1. 이미지가 표시되지 않아요
**A**: 파일 경로를 확인하세요
```html
<!-- 올바른 경로 -->
<img src="images/hackathon.jpg">

<!-- 잘못된 경로 -->
<img src="hackathon.jpg">  ❌
<img src="/images/hackathon.jpg">  ❌
```

### Q2. 이미지가 찌그러져 보여요
**A**: `object-fit: cover` 속성을 추가하세요
```html
<img src="images/hackathon.jpg" style="object-fit: cover;">
```

### Q3. 이미지가 너무 커요
**A**: 온라인 압축 도구로 파일 크기를 줄이세요
- TinyPNG: https://tinypng.com/
- Squoosh: https://squoosh.app/

### Q4. 실제 사진이 없어요
**A**: 임시로 Unsplash 이미지를 사용하되, 반드시 실제 사진으로 교체하세요

---

## 📞 추가 도움이 필요하신가요?

이미지 추가 중 문제가 발생하면 README.md를 참고하거나 문의해주세요!

---

**제작일**: 2026-02-05  
**버전**: 1.0.0

✨ **완성도 높은 현장 스케치를 위해 고품질 이미지를 준비해주세요!**
