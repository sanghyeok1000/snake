# 🐍Snake Game

## 소개
- 이 프로젝트는 클래식 스네이크 게임을 터미널에서 실행할 수 있도록 C++와 ncurses 라이브러리를 사용하여 구현한 것입니다. 
- 사용자는 방향키를 사용하여 스네이크를 이동시키며, 아이템을 먹어 점수를 획득하고 미션을 완료하여 다음 스테이지로 넘어갑니다.

## 사용 언어 및 라이브러리
- **사용 언어:** C++
- **사용 라이브러리:** ncurses

## 소스 코드 컴파일
g++ -std=c++11 -o snake snake.cpp -lncurses

## 실행방법
./snake

## 1️⃣ 게임 방법
이동
방향키: 스네이크를 상하좌우로 이동시킵니다.
반대 방향키: 스네이크의 현재 진행 방향과 반대 방향의 방향키를 누르면 게임이 종료됩니다.

## 2️⃣ 아이템
- '+' (Growth Item): 획득 시 스네이크의 길이가 1 증가합니다.
- '-' (Poison Item): 획득 시 스네이크의 길이가 1 감소합니다. 
                  스네이크의 길이가 3 이하로 줄어들면 게임이 종료됩니다.
- '*' (Special Item): 획득 시 보너스 점수를 얻고, 1초 동안 게임 속도가 느려집니다.

## 3️⃣ 게이트
- 'O' (Gate): 한 쌍으로 존재하며, 한쪽 게이트로 들어가면 반대쪽 게이트로 나옵니다. 
- 게이트는 5초마다 위치가 변경되며, 스네이크가 통과 중일 때는 변경되지 않습니다.

## 4️⃣ 미션
- 각 스테이지마다 주어지는 미션을 완료하면 다음 단계로 넘어갑니다.
- 예시 미션:
  ##### 스네이크 길이 10 이상 도달
  ##### 5개의 Growth Item 획득 
  ##### 2개 이하의 Poison Item 획득
  ##### 1회 이상 게이트 통과

## 5️⃣ 프로젝트 구조
- game.cpp: 게임의 주요 로직을 포함한 소스 코드 파일.
- snake: 컴파일된 실행 파일.

## 팀원
- 20201916 박상혁
- 20202086 백승렬
