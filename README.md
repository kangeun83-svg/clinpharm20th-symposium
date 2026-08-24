# AI 신약규제과학 학술심포지엄 웹사이트

서울성모병원 임상약리과 20주년 개소 기념 심포지엄 안내 페이지입니다.
정적 HTML 한 장으로 구성되어 있어 GitHub Pages로 바로 배포할 수 있습니다.

## 폴더 구성

```
index.html          메인 페이지 (모든 CSS/JS 포함)
assets/poster.pdf    포스터 원본 PDF (다운로드 링크로 연결)
assets/poster-web.jpg 웹 표시용 포스터 이미지
assets/poster-thumb.jpg 썸네일 (필요시 사용)
assets/qr.png        참가신청(홈) 페이지로 연결되는 QR코드
assets/qr-poster.png 포스터 PDF로 바로 연결되는 QR코드
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

- **간단한 텍스트/글자 수정** (오타, 띄어쓰기, 문구 변경): 저장소에서 `index.html` 클릭 → 연필(✏️) 아이콘 클릭 → `<`와 `>` 사이의 태그는 건드리지 말고, 그 사이에 있는 글자만 고치기 → 맨 아래 **Commit changes**.
  - 예: `<h3>일시</h3>` 에서 "일시"라는 글자만 바꾸는 건 안전하지만, `<h3>`나 `</h3>` 같은 부분을 지우면 화면이 깨질 수 있어요.
  - 확신이 안 서면 무엇을 바꾸고 싶은지 알려주세요. 파일을 고쳐서 다시 전달해드릴게요.
- **포스터 교체**: `assets/poster.pdf`와 `assets/poster-web.jpg`를 새 파일로 교체 업로드 (같은 파일명으로 업로드하면 덮어쓰기 됩니다)
- **참가신청 구글폼 주소 변경**: `index.html` 안에 `forms.gle/...` 링크가 여러 곳(상단 버튼, 첫 화면, 참가신청 섹션, 하단, 우측 하단 버튼)에 반복돼서 하나라도 빠뜨리면 링크가 서로 달라져요. 직접 고치기보다는, 새 구글폼 주소를 전달해주시면 한 번에 전체 교체해서 파일을 다시 드리는 방법을 권장합니다.

## QR코드 2종

- `assets/qr.png` — 스캔하면 웹사이트 첫 화면(홈)으로 이동
- `assets/qr-poster.png` — 스캔하면 포스터 PDF가 바로 열림 (인쇄물에 넣기 좋음)

인쇄용 포스터 디자인 파일(원본 디자인 툴)에 QR 이미지를 삽입한 뒤 PDF로 다시 내보내면 실물 포스터에도 QR을 넣을 수 있습니다.
