[← 전체 포트폴리오](../README.md)

# Cube Runner

![Cube Runner 게임 화면](../images/cube-runner.png)

| 항목 | 내용 |
| --- | --- |
| 기술 | C++, DirectX 11 |
| 기간 · 팀 | 3개월 · 프로그래머 2명 |
| 담당 | 게임 프레임워크, 콘텐츠 |
| 코드 | [CurtainCall3D](https://github.com/FinalPoopHead/CurtainCall3D) |
| 원본 기록 | [Notion · Cube Runner](https://piros.notion.site/Cube-Runner-28244c77edc34b8aa412955fa62e70cb) |

종이비행기로 장애물을 피하는 게임에서 출발해, 지뢰로 큐브를 제거하는 퍼즐 게임으로 방향을 바꾼 프로젝트입니다. 프로젝트 전체에서는 수학 라이브러리, 트위닝, 운영체제 추상화, 렌더러 추상화, 게임 프레임워크를 구현했습니다. 이 가운데 제가 맡은 범위는 **게임 프레임워크와 콘텐츠**입니다.

## 설계 사례: 수학 연산과 빌드 구성

프로젝트의 수학 라이브러리는 1~4차원 벡터와 4×4 행렬을 지원합니다. 원본 기록에서는 Debug 구성에서 SIMD가 더 느리게 동작한 경험을 바탕으로, **Release에서는 SSE 기반 SIMD, Debug에서는 SISD**를 사용하는 선택을 설명했습니다.

이는 해당 프로젝트에서 관찰한 결과에 따른 선택입니다. 빌드 조건을 구분한 사례로 소개하며, 모든 환경에서 동일한 성능 차이가 발생한다는 의미는 아닙니다.

[← 전체 포트폴리오](../README.md)
