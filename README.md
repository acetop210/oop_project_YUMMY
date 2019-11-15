# 2019-2 객체지향 프로그래밍 프로젝트 - YUMMY
구성원: **2-1 염주찬** | **2-4 김동혁** | **2-5 이승민**

## 1. 주제
학생들이 즐겨하는 단체 게임인 `마피아` 게임을 파이썬으로 만들어 보자.

## 2. 동기
우리가 즐겨 했던 게임을 온라인 상으로 구현 한다면 언제든지 친구들이 즐길 수 있을 것 같았다. 또한 턴제 게임이며 플레이어들의 직업과 역할이 뚜렷하게 나누어 지기 때문에 객체지향 프로그램의 장점을 최대한 살릴 수 있을 것이라고 생각했기 때문이다.

## 3. 프로그램 사용 대상
학생, 교사 남녀노소와 관계없이 즐거운 게임을 즐기고 싶은 사람들

## 4. 목적
  * 많은 사람들이 한꺼번에 즐길 수 있는 게임인 마피아를 제작한다. 인원수는 8명이며 인원들의 2명은 마피아 직업으로 배정받고, 1명은 경찰, 1명은 의사로 배정을 한다. 나머지는 일반 시민이다. 각 직업마다 특수한 능력이 있으며 일반팀이 승리하기 위해서는 마피아를 찾아내야 하며, 마피아가 승리하기 위해서는 일반인(시민,경찰,의사)들을 제거해야 한다. 
  * 위 게임을 통해 자신의 직업을 속일 수 있는 능력과 수많은 대화 사이에서 다른 사람의 직업을 추론해 낼 수 있는 능력을 기를 수 있을 것이라고 기대한다. 또한 무료한 학생들에게 짧은 시간 동안 할 수 있는 여가거리를 제공해줄 수 있다.

## 5. 주요기능
   1) 게임 시작
      - 서버에 여러 명의 클라이언트(플레이어)가 접속하고, 그 수가 8명이 되는 순간 게임이 시작된다.
   2) 투표
      - 1인당 1개의 투표권을 가진다.
      - 1차 투표에서는 처형 후보자를 뽑는다. (ID 제출)
      - 1차 투표 직후에는 후보자의 변론 시간이 주어진다.
      - 후보자의 변론이 끝나면 처형 찬반 투표가 이루어진다. (과반수 찬성의 경우 처형)
   3) 직업별 활동
      - 밤이 되면 직업별 특성에 따른 활동을 하게 된다.
      - 밤이 되면 채팅이 `같은 직업군`끼리의 소통으로 바뀌게 된다.

## 6. 프로젝트 핵심
   1) 시간
      - 낮과 밤의 시간 제한을 설정하고 이를 게임 상에서 구현해야 한다.
      - 투표의 시간 제한을 설정하고 이를 게임 상에서 구현해야 한다.
   2) 채팅
       - 채팅을 통해 판단의 근거를 얻는 게임으로, 채팅 기능을 완벽히 구현해야한다.
       - 밤에는 반드시 같은 직업군 사이의 채팅만 가능하도록 구현해야한다.
       - 시민들은 밤에 채팅을 할 수 없다.
   3) 접속
       - 8명이 들어오면 게임을 시작해야한다.
       - 8명이 들어온 상태에서는 추가적인 접속을 차단해야한다.
       - 클라이언트의 ID를 설정해야한다.

## 7. 구현에 필요한 라이브러리나 기술
   + pygame: GUI 구현 용도
   + random : npc의 움직임 제어

## 8. **분업 계획**
+ 염주찬 : 조종하고 동적인 캐릭터들과 상호작용하는 객체 설계(컵밥, 함정, 사감선생님)
+ 이승민 : 실제로 움직이는 캐릭터들에 대한 설계(4기, 5기)
+ 김동혁 : 완성된 게임을 파이게임으로 이식, 및 객체 설계 도움

## 9. 기타


<hr>

#### readme 작성관련 참고하기 [바로가기](https://heropy.blog/2017/09/30/markdown/)

#### 예시 계획서 [[예시 1]](https://docs.google.com/document/d/1hcuGhTtmiTUxuBtr3O6ffrSMahKNhEj33woE02V-84U/edit?usp=sharing) | [[예시 2]](https://docs.google.com/document/d/1FmxTZvmrroOW4uZ34Xfyyk9ejrQNx6gtsB6k7zOvHYE/edit?usp=sharing) | [[예시 3]](https://github.com/goldmango328/2018-OOP-Python-Light) | [[예시4]](https://github.com/ssy05468/2018-OOP-Python-lightbulb) | [[모두보기]](https://github.com/kadragon/oop_project_ex/network/members)
