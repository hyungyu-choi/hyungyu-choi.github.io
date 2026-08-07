# images/ 폴더 가이드

이미지 파일을 아래 경로/이름에 맞춰 넣기만 하면 `index.html` 수정 없이 바로 반영됩니다.
파일이 없는 동안에는 `placeholder-*.svg` 가 대신 표시되므로 레이아웃이 깨지지 않습니다.

## papers/ — 논문 figure (Publication 왼쪽)
권장: 가로형(4:3 ~ 16:9), 가로 800px 이상

| 파일명 | 논문 |
|---|---|
| `papers/goal.png` | GOAL (CVPR 2025) |
| `papers/fast-goal.png` | FAST-GOAL (IEEE TIP) |
| `papers/viral.png` | VIRAL (ICLR Workshop 2026) |
| `papers/tufs.png` | TuFS (Under Review) |
| `papers/techart.png` | Detailed Caption Processing (TechArt) |

## logos/ — 저자 소속 로고 (Publication 오른쪽 아래)
권장: **가로가 긴 로고**, 높이 100~150px, 배경 투명 PNG (또는 SVG)
표시 높이는 36px로 고정되고 가로는 비율에 맞춰 자동 조정됩니다.

| 파일명 | 위치 |
|---|---|
| `logos/goal-1.png`, `logos/goal-2.png` | GOAL |
| `logos/fast-goal-1.png`, `logos/fast-goal-2.png` | FAST-GOAL |
| `logos/viral-1.png`, `logos/viral-2.png` | VIRAL |
| `logos/tufs-1.png`, `logos/tufs-2.png` | TuFS |
| `logos/techart-1.png` | TechArt |

로고 개수를 바꾸려면 `index.html` 의 `.affiliation-logos` 안에서
`<img class="affil-logo" ...>` 줄을 복사하거나 지우면 됩니다.

## edu/ — 학교 로고 (Education 왼쪽)
권장: 정사각형에 가까운 이미지, 200x200px 이상, 배경 투명 PNG

| 파일명 | 위치 |
|---|---|
| `edu/cau.png` | Chung-Ang University (M.S. / B.S. 두 항목이 공유) |

## gallery/ — 갤러리 이미지
권장: 가로형 4:3, 가로 800px 이상 (`object-fit: cover` 로 잘려서 표시됨)

`gallery/01.jpg`, `gallery/02.jpg`, `gallery/03.jpg` …
항목을 늘리려면 `index.html` 의 `<figure class="gallery-item">` 블록을 복사하세요.

## media/ — (선택) 유튜브 커스텀 썸네일
유튜브 항목은 기본적으로 `https://img.youtube.com/vi/<VIDEO_ID>/hqdefault.jpg` 를
자동으로 불러옵니다. 직접 만든 썸네일을 쓰고 싶을 때만 이 폴더를 사용하고
`index.html` 의 `<img src="...">` 경로를 바꿔주세요.

## placeholder-*.svg
직접 수정할 필요 없는 대체 이미지입니다. 삭제하지 마세요.
