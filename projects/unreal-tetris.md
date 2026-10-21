[← 전체 포트폴리오](../README.md)

# Unreal Tetris

![Unreal Engine으로 제작한 Tetris](../images/tetris-unreal.png)

| 항목 | 내용 |
| --- | --- |
| 기술 | C++, Unreal Engine |
| 기간 · 팀 | 1주 · 개인 개발 |
| 목적 | Unreal Engine의 구조·모듈·에디터 사용과 생성자에서의 메시 설정 학습 |
| 코드 | [HelloUnreal](https://github.com/PinkBourbon/HelloUnreal) |
| 원본 기록 | [Notion · Tetris](https://piros.notion.site/20e432cf43c280c5ae18d9dfc1c66b14) |

작은 게임을 완성하는 과정을 통해 Unreal Engine의 기본 구조를 익혔습니다. 게임 진행과 입력, 화면 표현을 다음 다섯 클래스로 나누었습니다.

| 클래스 | 기반 클래스 | 역할 |
| --- | --- | --- |
| `ATetrisGameMode` | `AGameModeBase` | 보드 생성 |
| `ATetrisBoard` | `AActor` | 보드 상태와 테트로미노 종류 관리, 카메라 생성 |
| `ATetrisCamera` | `AActor` | 직교 투영 카메라 |
| `ATetromino` | `AActor` | 테트로미노 종류·상태에 따른 표현 |
| `ATetrisPlayerController` | `APlayerController` | `EnhancedInputComponent`를 통한 입력 처리 |

각 클래스의 책임을 정리하면서 엔진이 제공하는 게임플레이 구조를 학습한 프로젝트입니다. 생성자에서 메시를 설정하는 방식도 함께 익혔습니다.

[← 전체 포트폴리오](../README.md)
