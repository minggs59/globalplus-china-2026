# 2026학년도 동계 글로벌플러스(중국) 안내 페이지

강남대학교 시니어비즈니스학과 · 강남대학교 국제협력팀의 글로벌플러스(중국) 프로그램 안내용 정적 웹사이트입니다.

## 포함 파일
- `index.html`: 모바일 반응형 안내 페이지
- `styles.css`: 화면 디자인 및 반응형 스타일
- `config.js`: 네이버폼 주소 설정
- `assets/`: 강남대학교 로고, 학생 배포용 계획안 PDF, 지원서 HWP 원본 및 PDF 미리보기

## 반영된 주요 일정
- 모집 및 서류 접수: 2026년 11월 24일(화)부터 11월 27일(금) 12:00까지
- 면접: 2026년 11월 27일(금) 15:00부터 예정
- 면접 대상자에게 개별 안내하며, 세부 시간과 장소는 별도 안내

계획안 PDF 2쪽의 모집 마감일 및 면접일을 수정했고, 지원서 PDF 미리보기 1쪽의 파견기간 연도 표기(2025→2026)를 수정했습니다. 단, 한글(HWP) 원본은 이 작업 환경에서 직접 수정할 수 없어 기존 파일을 유지했습니다. HWP 원본을 배포하기 전 한글 프로그램에서 파견기간의 `2025학년도 동계방학`을 `2026학년도 동계방학`으로 수정해야 합니다.

참고: 기존 계획안에는 11월 27일(금) 1차 사전교육 일정도 기재되어 있습니다. 면접과 같은 날 진행할지, 시간 변경이 필요한지 확인 후 계획안 최신본에 반영해 주세요.

## 배포 전 반드시 할 일
1. `config.js`의 `applicationFormUrl`에 실제 네이버폼 주소를 입력합니다.
2. 문의 담당자 이메일 및 연락처가 확정되면 `index.html`의 문의 안내 영역에 반영합니다.
3. 위의 HWP 원본 연도 표기를 수정하고 최신본으로 교체합니다.
4. 모바일 환경에서 PDF 미리보기 및 HWP 다운로드를 확인합니다.

## GitHub Pages 배포
1. GitHub 저장소 `minggs59/globalplus-china-2026`을 엽니다.
2. `Add file` → `Upload files`를 선택합니다.
3. 이 ZIP을 컴퓨터에서 압축 해제한 뒤, 폴더 안의 **모든 파일과 `assets` 폴더**를 저장소 루트로 끌어다 놓습니다. `index.html`이 저장소 최상위에 있어야 합니다.
4. `Commit changes`를 눌러 업로드합니다.
5. 저장소 `Settings` → `Pages` → `Build and deployment`에서 `Deploy from a branch`, Branch `main`, Folder `/(root)`를 선택하고 저장합니다.
6. 배포가 완료되면 `https://minggs59.github.io/globalplus-china-2026/` 주소에서 확인합니다.

## Vercel로 배포할 경우
1. Vercel에서 Add New → Project를 선택하고 GitHub 저장소 `globalplus-china-2026`을 Import 합니다.
2. Framework Preset은 `Other`, Build Command는 비우고 Output Directory는 `.`로 설정합니다.
3. Deploy를 누릅니다.

이 사이트는 별도 빌드 과정이 없는 정적 HTML/CSS/JS입니다. 현재 GitHub 연동은 저장소 읽기까지 확인됐으나, 파일 쓰기 요청은 권한 오류(403)로 거부되었습니다. 따라서 아래 ZIP을 이용해 GitHub 웹 화면에서 파일을 업로드해야 합니다.
