### 프리코스 과제 가이드
---

- 프리코스 과제 가이드 
- https://github.com/woowacourse/woowacourse-docs/tree/main/precourse#%EC%A0%9C%EC%B6%9C-%EA%B0%80%EC%9D%B4%EB%93%9C
- 과제를 어떻게 제출하는지의 과정으로, 크게 git 을 fork, clone , 브랜치 생성, ide로 import,본인 원격 저장소에 올리는 과정, 그리고 pull request 까지를 다루고 있다. 차근차근 따라해 보자!


- 프로젝트를 자신의 계정으로 fork하기
  - 우테코 저장소에 쓰기 권한이 없으니 fork 해온 후 내 계정에서 코드를 구현하도록 하겠다.
  - **fork** 는 저장소를 자신의 계정으로 복사해오는 것.

- fork 한 저장소를 컴퓨터로 clone 하기
  - fork 한 저장소를 이제 코드를 쓰고, 수정하기 위해 내 pc로 복사하자. 
  - git에서 많이 해본거라 괜찮다.
  
- 기능 구현을 위한 브랜치 생성
  - 클론해온 것에서 바로 작업을 하지 않고, 나의 작업만을 하기 위해 따로 브랜치를 만들어 그 브랜치에서만 작업할 것이다.
  - 확실한건 아니지만 협업 때는 각자 브랜치에서 작업을 하고, 머지를 하기 때문에 미리 연습해보는 의미이지 않겠다 싶다.
  - branch 관련 명령어.
    - 브랜치 생성 : ```git branch 새브랜치이름```
    - 브랜치 생성과 동시에 체크아웃 : ```git branch -b 새브랜치이름```
    - 브랜치 목록 조회 : ```git branch```
  - branch 이동 명령어.
    - 어느 브랜치로 가겠다 : ```git switch 브랜치이름  ```
  
  - git branch -b 를 통해 miffyKing 이란 이름의 브랜치를 새로 만들었다. 그러고 git 홈페이지에서 새로 브랜치가 만들어 졌는지 확인하면 아직 반영이 안되어 있다. 새 브랜치에서 작업 후 push 까지해야 miffyKing 브랜치가 보일 것이다. 예전에 사촌동생 과제를 도와주다가 알게된 사실이다!
  
  ![image](https://user-images.githubusercontent.com/87696004/197821898-1c6638fe-3a7d-425e-9f01-c88a494a30da.png)

- 통합 개발 환경 (IDE) 로 가져오기.
  - 내가 이용할 ide로 가져온다. 난 인텔리제이를 사용할것이다.
  - 아무리 씹 찾아잮ㅕ도 import project가 없다. 걍 open project로 열면 gradle issue라고 나온다. 속상하다;;;;;



- 수정후 commit, push 하기
  - git add . 
  - git commit -m "   "
  - 까지는 똑같이 했는데
  - 실수로 git push 만 하고 안된다 판단해 
  - ``` git push --set-upstream origin miffyKing ```
  - 이 명령을 갈겨 push 했다. 내일 어차피 다시 할 땐 꼭 ``` git push origin miffyKing ``` 으로 올리겠다.


- pull request 보내기