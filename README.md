# LOLDOV Frontend

| 파일 | 설명 |
| --- | --- |
| `coach/index.html` | 코칭 웹사이트 화면. 리플레이 영상 업로드(끌어다 놓기, 48MB 조각 전송·재시도), 분석 진행률, 분석 기록·예시 경기, 코칭 리포트(총평·개선점·연습 과제·구간별 격차·타임라인 차트·장면별 코칭과 프레임), 코치에게 질문하기 |
| `report/template.html` | 개발 영상 분석 결과를 모아 보는 정적 리포트의 틀. AI 저장소의 `python -m report.build_site`가 데이터를 넣어 `AI/results/site/index.html`을 만든다 |

빌드 도구 없이 HTML·CSS·JS 한 파일로 되어 있고, 라이트·다크 테마를 지원한다.

## 실행

`coach/index.html`은 [Backend](https://github.com/LOLDOV/Backend) 서버가 `/`로 제공한다 (같은 주소의 `/api/...` 호출).
AI·Backend·Frontend 저장소를 같은 상위 폴더에 나란히 클론한 뒤 Backend README대로 서버를 켜고 http://localhost:8000 에 접속한다.
