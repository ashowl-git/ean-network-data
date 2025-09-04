# 🌐 EAN 네트워크 데이터 - GitHub Pages 호스팅

## 📁 파일 구성

```
github-pages-hosting/
├── index.html                    # 메인 웹페이지 (최적화된 버전)
├── ean_full_network_data.json   # JSON 데이터 파일 (분리된 버전)
└── README.md                    # 설정 가이드
```

## 🚀 GitHub Pages 호스팅 방법

### 1단계: GitHub 저장소 생성
1. GitHub에 로그인 후 새 저장소 생성
2. 저장소 이름: `ean-network-data` (또는 원하는 이름)
3. Public으로 설정 (GitHub Pages는 Public 저장소에서만 무료)

### 2단계: 파일 업로드
1. 저장소에서 "Upload files" 클릭
2. 이 폴더의 모든 파일을 드래그 앤 드롭:
   - `index.html`
   - `ean_full_network_data.json`
   - `README.md`

### 3단계: GitHub Pages 활성화
1. 저장소 Settings → Pages
2. Source: "Deploy from a branch"
3. Branch: `main` 또는 `master` 선택
4. Folder: `/ (root)` 선택
5. Save 클릭

### 4단계: 접속 확인
- 약 5-10분 후 다음 주소로 접속:
- `https://[사용자명].github.io/[저장소명]/`

## ⚡ 성능 최적화 특징

### 🔄 비동기 로딩
- JSON 데이터를 별도 파일로 분리
- `fetch()` API를 사용한 비동기 로딩
- 로딩 스피너와 진행 상태 표시

### 📊 실시간 통계
- 총 노드 수, 링크 수 표시
- 데이터 크기와 로딩 시간 측정
- 브라우저 콘솔에서 상세 로그 확인

### 📱 반응형 디자인
- 모바일, 태블릿, 데스크톱 지원
- 현대적인 카드 기반 UI
- 접근성을 고려한 디자인

## 🛠️ 개발자 도구

### 브라우저 콘솔에서 데이터 접근
```javascript
// 로드된 네트워크 데이터 가져오기
const data = window.getNetworkData();
console.log('노드 수:', data.nodes.length);
console.log('링크 수:', data.links.length);
```

### 성능 모니터링
- F12 → Network 탭에서 로딩 시간 확인
- Console 탭에서 상세 로그 확인
- Performance 탭에서 성능 분석

## 🔧 커스터마이징

### CSS 스타일 수정
`index.html` 파일의 `<style>` 섹션에서 디자인 변경 가능

### JavaScript 기능 추가
`<script>` 섹션에서 추가 기능 구현:
- 네트워크 그래프 시각화 (D3.js, vis.js 등)
- 데이터 필터링 및 검색
- 통계 차트 추가

## 📈 확장 아이디어

1. **네트워크 그래프 시각화**
   - D3.js force-directed graph
   - vis.js network diagram
   - Cytoscape.js

2. **데이터 분석 도구**
   - 노드 중심성 분석
   - 클러스터 분석
   - 경로 분석

3. **인터랙티브 기능**
   - 노드 검색 및 하이라이트
   - 필터링 옵션
   - 데이터 내보내기

## 🐛 문제 해결

### CORS 에러 발생 시
- GitHub Pages에서는 자동으로 해결됨
- 로컬 테스트 시: `python -m http.server 8000`

### 파일 크기 제한
- GitHub 파일 크기 제한: 100MB
- 현재 JSON 파일: 약 5.3MB (문제없음)

### 로딩 속도 개선
- JSON 파일 압축 (gzip)
- CDN 사용 고려
- 데이터 청크 분할 로딩

## 📞 지원

문제가 발생하면 다음을 확인하세요:
1. 브라우저 콘솔에서 에러 메시지 확인
2. 네트워크 탭에서 파일 로딩 상태 확인
3. GitHub Pages 설정이 올바른지 확인

---
**최적화된 웹 성능으로 빠르고 안정적인 데이터 시각화를 경험하세요! 🚀** 