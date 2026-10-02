# 부산·경남 미술 이슈보드

부산·경남 미술학원 소식, 2027 미대입시 대학 공지·전형표, 초·중·고 미술·디자인 공모전을 한곳에 모은 정적 사이트입니다.

- 사이트: https://dbsrugk.github.io/busan-art-issue-board/
- 화면: `#news` 학원 소식 · `#admission` 미대입시 · `#contest` 공모전

## 구성

| 파일 | 내용 |
| --- | --- |
| `index.html` | 화면·스타일·스크립트 전체 (빌드 없음) |
| `data/board.json` | `issues`(학원 소식), `admission`(대학 공지), `contests`(공모전), `officialUrls`, `academies`, `updatedAt` |
| `data/programs.json` | 대학별 전형표 (508개 전형) |

## 데이터 수정

1. `data/board.json`에서 해당 배열에 항목을 추가·수정합니다.
2. 날짜는 `YYYY.MM.DD`(소식·공지) 또는 `YYYY-MM-DD`(공모전 `startDate`/`endDate`) 형식입니다. 공모전 마감 시각이 정확히 있으면 `endAt`에 `2026-10-18T23:59:59+09:00`처럼 넣습니다.
3. `updatedAt`을 갱신 날짜로 바꿉니다.
4. 커밋하면 GitHub Pages가 1~2분 안에 반영합니다.

공모전 접수 상태와 D-day는 열람 시점(한국 시간) 기준으로 자동 계산됩니다. 입시·공모전 정보는 반드시 대학·주최기관 원문으로 최종 확인하세요.
