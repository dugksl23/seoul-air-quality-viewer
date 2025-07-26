# seoul-air-quality-viewer

# 🏙️ 서울시 대기질 정보 조회기

![Air Quality Banner](https://img.shields.io/badge/Project-Seoul%20Air%20Quality-blue?style=for-the-badge&logo=github)
![Language](https://img.shields.io/badge/Language-HTML%2FCSS%2FJavaScript-orange?style=for-the-badge&logo=javascript)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge&logo=opensourceinitiative)

서울시의 시간별 대기질 정보를 간편하게 조회하고 엑셀 파일로 다운로드할 수 있는 웹 애플리케이션입니다. 서울시 열린데이터광장의 대기질 데이터를 활용하여 특정 년도, 월/분기, 일자, 시간, 측정소별 대기 데이터를 확인하고 분석할 수 있습니다.

## ✨ 주요 기능

* **년도, 월/분기 선택**: 원하는 기간의 대기질 데이터를 조회합니다.
* **세부 일자 및 시간 선택**: 특정 날짜나 시간대의 데이터를 집중적으로 조회할 수 있습니다.
* **측정소별 필터링**: 서울시 25개 구별 측정소 데이터를 선택하여 확인합니다.
* **표 형식 데이터 표시**: 조회된 데이터를 깔끔한 테이블 형태로 보여줍니다.
* **엑셀(Excel) 다운로드**: 조회된 모든 데이터를 `.xlsx` 형식으로 다운로드하여 오프라인에서 활용할 수 있습니다. (측정소명은 '서울시구'로 자동 변환)

## 🚀 시작하기

이 애플리케이션은 순수 HTML, CSS, JavaScript로 구성된 정적 웹 페이지입니다. 별도의 서버 설정 없이 웹 브라우저에서 바로 실행할 수 있습니다.

### 💻 로컬에서 실행하기

1.  이 저장소를 클론(Clone)하거나 ZIP 파일로 다운로드합니다:
    ```bash
    git clone [https://github.com/YOUR_USERNAME/seoul-air-quality-viewer.git](https://github.com/YOUR_USERNAME/seoul-air-quality-viewer.git)
    cd seoul-air-quality-viewer
    ```
    (여기서 `YOUR_USERNAME`은 당신의 GitHub 사용자명입니다.)

2.  `index.html` 파일을 웹 브라우저로 엽니다. (파일을 더블 클릭하거나, 웹 브라우저에 드래그 앤 드롭).

### 🌐 온라인에서 접속하기 (GitHub Pages)

이 프로젝트는 GitHub Pages를 통해 배포될 예정입니다. 배포가 완료되면 다음 링크에서 직접 접속할 수 있습니다:

[https://YOUR_USERNAME.github.io/seoul-air-quality-viewer/](https://YOUR_USERNAME.github.io/seoul-air-quality-viewer/)
(위 링크에서 `YOUR_USERNAME`을 본인의 GitHub 사용자명으로 변경하세요.)

## 🛠️ 기술 스택

* **HTML5**: 웹 페이지 구조
* **CSS3**: 스타일링
* **JavaScript (ES6+)**: API 통신 및 데이터 처리
* **xlsx.js**: 엑셀 파일 생성 및 다운로드 (CDN 사용)
* **서울시 열린데이터광장 API**: `TimeAverageAirQuality` 서비스

## 🔑 API 키 설정

이 애플리케이션은 서울시 열린데이터광장 API를 사용합니다. `index.html` 파일 내에 API 키를 설정해야 합니다.

```javascript
const API_KEY = 'YOUR_API_KEY_HERE'; // 실제 발급받은 API 키로 교체
