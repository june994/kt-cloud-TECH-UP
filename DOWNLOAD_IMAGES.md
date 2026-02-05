# 이미지 다운로드 가이드

이 파일은 현재 사용 중인 이미지들을 다운로드하는 방법을 안내합니다.

## 📥 이미지 다운로드 URL 목록

### 로고
```
https://www.genspark.ai/api/files/s/JicupQXg
→ 다운로드 후 images/logo.png로 저장
```

### 행성 이미지
```
https://www.genspark.ai/api/files/s/gYiq17mb → images/planet1.png
https://www.genspark.ai/api/files/s/xY8BtxVl → images/planet2.png
https://www.genspark.ai/api/files/s/eGD1zDZC → images/planet3.png
https://www.genspark.ai/api/files/s/yXzLuEb4 → images/planet4.png
https://www.genspark.ai/api/files/s/T1YG5TqA → images/planet5.png
https://www.genspark.ai/api/files/s/UanOP8YE → images/planet6.png
```

### 갤러리 이미지 (현장 스케치 9개)
```
https://www.genspark.ai/api/files/s/0txqz82t → images/gallery1.jpg (WARM UP DAY 단체)
https://www.genspark.ai/api/files/s/xIn6MnnR → images/gallery2.jpg (현직자 특강)
https://www.genspark.ai/api/files/s/OsSeCyTP → images/gallery3.jpg (질문하는 교육생)
https://www.genspark.ai/api/files/s/8pDHimM0 → images/gallery4.jpg (웃는 교육생들)
https://www.genspark.ai/api/files/s/jljU5J7I → images/gallery5.jpg (응원하는 교육생들)
https://www.genspark.ai/api/files/s/EJF7AQpQ → images/gallery6.jpg (집중하는 교육생)
https://www.genspark.ai/api/files/s/zjWTa32I → images/gallery7.jpg (럭키드로우 이벤트)
https://www.genspark.ai/api/files/s/bky3YoRj → images/gallery8.jpg (박수치는 교육생들)
https://www.genspark.ai/api/files/s/WkZVuq4l → images/gallery9.jpg (단체 사진)
```

## 🔧 다운로드 방법

### 방법 1: 브라우저에서 수동 다운로드

1. 위 URL을 브라우저에서 하나씩 열기
2. 우클릭 → "다른 이름으로 이미지 저장"
3. 파일명을 해당하는 이름으로 변경 (예: `logo.png`, `gallery1.jpg` 등)
4. `images/` 폴더에 저장

### 방법 2: wget 사용 (Mac/Linux)

```bash
# images 폴더 생성
mkdir -p images

# 로고 다운로드
wget -O images/logo.png https://www.genspark.ai/api/files/s/JicupQXg

# 행성 이미지 다운로드
wget -O images/planet1.png https://www.genspark.ai/api/files/s/gYiq17mb
wget -O images/planet2.png https://www.genspark.ai/api/files/s/xY8BtxVl
wget -O images/planet3.png https://www.genspark.ai/api/files/s/eGD1zDZC
wget -O images/planet4.png https://www.genspark.ai/api/files/s/yXzLuEb4
wget -O images/planet5.png https://www.genspark.ai/api/files/s/T1YG5TqA
wget -O images/planet6.png https://www.genspark.ai/api/files/s/UanOP8YE

# 갤러리 이미지 다운로드
wget -O images/gallery1.jpg https://www.genspark.ai/api/files/s/0txqz82t
wget -O images/gallery2.jpg https://www.genspark.ai/api/files/s/xIn6MnnR
wget -O images/gallery3.jpg https://www.genspark.ai/api/files/s/OsSeCyTP
wget -O images/gallery4.jpg https://www.genspark.ai/api/files/s/8pDHimM0
wget -O images/gallery5.jpg https://www.genspark.ai/api/files/s/jljU5J7I
wget -O images/gallery6.jpg https://www.genspark.ai/api/files/s/EJF7AQpQ
wget -O images/gallery7.jpg https://www.genspark.ai/api/files/s/zjWTa32I
wget -O images/gallery8.jpg https://www.genspark.ai/api/files/s/bky3YoRj
wget -O images/gallery9.jpg https://www.genspark.ai/api/files/s/WkZVuq4l
```

### 방법 3: curl 사용 (Windows/Mac/Linux)

```bash
# images 폴더 생성
mkdir images

# 로고 다운로드
curl -o images/logo.png https://www.genspark.ai/api/files/s/JicupQXg

# 행성 이미지 다운로드
curl -o images/planet1.png https://www.genspark.ai/api/files/s/gYiq17mb
curl -o images/planet2.png https://www.genspark.ai/api/files/s/xY8BtxVl
curl -o images/planet3.png https://www.genspark.ai/api/files/s/eGD1zDZC
curl -o images/planet4.png https://www.genspark.ai/api/files/s/yXzLuEb4
curl -o images/planet5.png https://www.genspark.ai/api/files/s/T1YG5TqA
curl -o images/planet6.png https://www.genspark.ai/api/files/s/UanOP8YE

# 갤러리 이미지 다운로드
curl -o images/gallery1.jpg https://www.genspark.ai/api/files/s/0txqz82t
curl -o images/gallery2.jpg https://www.genspark.ai/api/files/s/xIn6MnnR
curl -o images/gallery3.jpg https://www.genspark.ai/api/files/s/OsSeCyTP
curl -o images/gallery4.jpg https://www.genspark.ai/api/files/s/8pDHimM0
curl -o images/gallery5.jpg https://www.genspark.ai/api/files/s/jljU5J7I
curl -o images/gallery6.jpg https://www.genspark.ai/api/files/s/EJF7AQpQ
curl -o images/gallery7.jpg https://www.genspark.ai/api/files/s/zjWTa32I
curl -o images/gallery8.jpg https://www.genspark.ai/api/files/s/bky3YoRj
curl -o images/gallery9.jpg https://www.genspark.ai/api/files/s/WkZVuq4l
```

## ✅ 다운로드 완료 확인

다운로드 완료 후 폴더 구조:

```
kt-techup-showcase/
├── index.html
├── README.md
├── .gitignore
└── images/
    ├── logo.png
    ├── planet1.png
    ├── planet2.png
    ├── planet3.png
    ├── planet4.png
    ├── planet5.png
    ├── planet6.png
    ├── gallery1.jpg
    ├── gallery2.jpg
    ├── gallery3.jpg
    ├── gallery4.jpg
    ├── gallery5.jpg
    ├── gallery6.jpg
    ├── gallery7.jpg
    ├── gallery8.jpg
    └── gallery9.jpg
```

총 16개 이미지 파일이 있어야 합니다.

## 🚀 GitHub 업로드

이미지 다운로드 후:

1. `images/` 폴더를 포함한 모든 파일을 GitHub에 업로드
2. GitHub Pages에서 정상적으로 이미지가 표시됨

## 💡 팁

- 이미지가 표시되지 않으면 파일명과 확장자를 다시 확인하세요
- 대소문자를 정확히 맞춰야 합니다 (gallery1.jpg ≠ Gallery1.jpg)
- 이미지가 없어도 웹사이트는 작동하지만 플레이스홀더가 표시됩니다
