# ARSimulationGame
## 내 취향을 알면 휘둘리지 않아

당신은 어떤 대학 생활을 보내고 계신가요? AR로 즐기는 좌충우돌 우당탕탕 와글와글 대학생활 시뮬레이션 게임! 카이스트 곳곳에 숨겨져 있는 AR 사물들을 찾아 교수심의 호감도를 높이고, 당신의 선택에 따라 달라지는 결말을 경험해보세요.

### Contributer
**박정은** 포스텍 컴퓨터공학과 @jjungnii  
**신의진** 카이스트 전산학부 @euijinshin  
**우다연** 성균관대 데이터사이언스융합전공 @yeonyeonn  

### 개발 툴

- Unity AR + 2D 씬
- ios 빌드

### AR 지도 씬

- Mapbox의 Maps SDK for Unity(WorldScaleAR) 사용하였다.
- AR 체크박스 클릭 시 휴대폰의 카메라를 이용한 AR 화면으로 전환된다.
    - 위도와 경도로 지정해둔 위치에 AR 오브젝트가 뜬다.
        - 기숙사(아름관): 침대
        - 오리연못: 거위
        - 도서관: 책
        - N1: 커피
        - 쪽문: 고기
    - AR 오브젝트를 터치할 시 해당 스토리가 진행된다.
- Map 체크박스 클릭 시 2D 지도 화면으로 전환된다.
    - GPS를 통해 현재 나의 위치가 지도 상에 표현된다.
    - 스크롤을 통해 지도 상의 내 위치를 확인할 수 있다.

### 2D 스토리 씬

- AR 씬에서 사물을 터치하면 해당 사물이 의미하는 장소의 스토리 씬이 전개된다.
- 씬에 등장하는 서로 다른 선택지들은 각각의 스토리를 가진다.
- 각 장소마다 데이터 파일을 생성하여 데이터 파일간의 이동으로 씬 전환을 구성하였다.
- Unity 애니메이션으로 씬 전환 및 이미지 팝업을 조절하였다.

### 게임 세부 설명

- 모종의 사건으로 갑자기 4학년 졸업반이 되어버린 새내기 주인공이 14일간의 대학생활을 펼치는 게임
- 교수님의 호감도를 높여 아름다운 대학생활 결말을 맺는 것이 목표이다.
- 카이스트 곳곳에 숨겨진 AR 사물을 찾아 터치하면 각 장소에서의 스토리가 진행된다.
- 카이스트 기숙사 ‘아름관'에서는 하루가 시작되고 마무리되며, 각 장소에서의 스토리를 끝내면 ‘아름관'으로 이동한 후 하루가 차감된다.
- 2D 스토리 씬에서 선택하는 선택지에 따라 체력과 교수님의 호감도가 변화한다.
- 체력이 0이 되면 게임이 끝난다.
- 14일이 지나면 교수님의 호감도에 따라 다른 결말이 뜬다.
