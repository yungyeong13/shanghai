# 상하이 지도 리스트 (웹앱)

## GitHub Pages에 올리는 법

1. GitHub에서 새 저장소(repository)를 만듭니다. 이름은 아무거나, **Public**으로 만드세요.
   (Private은 GitHub Pages가 유료 플랜에서만 동작합니다.)
2. 이 폴더의 파일 6개를 저장소 최상단에 그대로 올립니다.
   index.html / manifest.webmanifest / sw.js / icon-192.png / icon-512.png / apple-touch-icon.png
   - 웹 화면에서 "Add file" → "Upload files"로 끌어다 놓으면 됩니다.
3. 저장소 Settings → 왼쪽 메뉴 Pages → Source를 "Deploy from a branch",
   Branch는 main / (root) 로 두고 Save.
4. 1~2분 뒤 https://<아이디>.github.io/<저장소이름>/ 주소가 생깁니다.

## 아이폰에 설치

1. **사파리**로 그 주소를 엽니다. (크롬 아님 — 사파리여야 설치가 됩니다.)
2. 목록이 다 뜰 때까지 기다린 뒤, 화면을 한 번 아래까지 훑어 내립니다.
3. 하단 공유 버튼 → "홈 화면에 추가" → 추가.
4. 홈 화면 아이콘으로 한 번 열어서 목록이 뜨는지 확인합니다.
5. **비행기 모드를 켜고** 다시 열어보세요. 그대로 열리면 성공입니다.

출국 전에 5번까지 꼭 확인하세요.

## 내용을 고치고 싶으면

index.html 안의 `const` 데이터가 아니라, 목록이 HTML로 직접 박혀 있습니다.
수정 후 다시 올릴 때는 sw.js 첫 줄의 `shanghai-v1`을 `shanghai-v2`처럼 바꿔야
아이폰이 옛날 캐시 대신 새 내용을 받아갑니다.
