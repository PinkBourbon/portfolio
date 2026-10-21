[← 전체 포트폴리오](../README.md)

# Dice or Die

![Dice or Die 게임 화면](../images/dice-or-die.png)

| 항목 | 내용 |
| --- | --- |
| 기술 | C++, DirectX2D — 원본 기록의 표기 |
| 기간 · 팀 | 3주 · 8명: 프로그래머 5명·아트 2명·기획 2명 |
| 담당 | 최적화, 일정 관리, 구조 설계 |
| 코드 | [원문에 연결된 저장소](https://github.com/PinkBourbon/GA4th2Q_Project) |
| 영상 | [YouTube · 실행 영상](https://www.youtube.com/watch?v=yRh2pDxUoFM) |
| 원본 기록 | [Notion · Dice or Die](https://piros.notion.site/Dice-or-Die-ba6d9b6115f042eb84f656eb61d1dd09) |

## 문제 해결: 공동 개발의 프로젝트 구조

이전 프로젝트에서 겪은 SVN 충돌을 계기로 개발자별 프로젝트·솔루션을 분리하는 구조를 적용했습니다. 빌드 의존성을 설정해 필요한 순서대로 빌드되도록 하고, 산출물 경로를 라이브러리 디렉터리로 연결했습니다.

협업 과정에서 각 개발자의 작업 단위를 나누면서 빌드 결과를 연결한 사례입니다. 원본의 팀 인원에는 불일치가 있으며, 연결된 저장소의 `main`에는 `RunAway/`, `RunAwayEngine/`, `RunAway.sln`이 있어 Dice or Die의 정확한 저장소·브랜치를 확인해야 합니다.

[← 전체 포트폴리오](../README.md)
