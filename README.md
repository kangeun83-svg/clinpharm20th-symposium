# AI 신약규제과학 학술심포지엄 웹사이트

서울성모병원 임상약리과 20주년 개소 기념 심포지엄 안내 페이지입니다.
정적 HTML 한 장으로 구성되어 있어 GitHub Pages로 바로 배포할 수 있습니다.

## 폴더 구성

```
index.html          메인 페이지 (모든 CSS/JS 포함)
assets/poster.pdf    포스터 원본 PDF (다운로드 링크로 연결)
assets/poster-web.jpg 웹 표시용 포스터 이미지
assets/poster-thumb.jpg 썸네일 (필요시 사용)
assets/qr.png        참가신청 페이지로 연결되는 QR코드
```

## GitHub Pages로 배포하는 방법 (터미널 없이, 웹에서만)

1. https://github.com/new 에서 새 저장소 생성
   - Repository name: `clinpharm20th-symposium` (원하는 이름으로 변경 가능)
   - Public 선택 → Create repository
2. 방금 만든 저장소 페이지에서 **Add file → Upload files** 클릭
3. 이 폴더 안의 `index.html`, `assets` 폴더를 그대로 끌어다 놓기 (drag & drop) → 맨 아래 **Commit changes**
4. 저장소 상단 **Settings → Pages** 이동
5. **Build and deployment → Source**를 `Deploy from a branch`로 설정
6. **Branch**를 `main` / `/ (root)`로 설정 후 **Save**
7. 1~2분 후 같은 화면 상단에 뜨는 주소로 접속 확인
   - 예: `https://kangeun83-svg.github.io/clinpharm20th-symposium/`

> ⚠️ 저장소 이름을 위 예시(`clinpharm20th-symposium`)와 다르게 만들면, 실제 접속 주소가 바뀌므로
> `assets/qr.png`의 QR코드가 가리키는 주소와 달라집니다. 이름을 바꿀 경우 QR코드를 다시 생성해야 합니다.

## 내용 수정하기

- 프로그램/연사/장소 등 텍스트 수정: `index.html`을 GitHub 웹에서 열고 연필(✏️) 아이콘으로 바로 편집 가능
- 포스터 교체: `assets/poster.pdf`와 `assets/poster-web.jpg`를 새 파일로 교체 업로드
- 참가신청 폼 주소 변경: `index.html` 내 `forms.gle/...` 링크를 모두 새 주소로 바꾸기 (Ctrl+F로 검색)

## QR코드를 인쇄 포스터에 넣는 방법

`assets/qr.png` 파일을 다운로드하여, 포스터 PDF 디자인 파일(원본 디자인 툴)에서 원하는 위치에 이미지로 삽입한 뒤 다시 PDF로 내보내면 됩니다.
