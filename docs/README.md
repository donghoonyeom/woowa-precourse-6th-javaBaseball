숫자 야구
-

- 시작 문구("숫자 야구 게임을 시작합니다.")
- 랜덤 숫자 변수 생성 : pickNumberInRange() 이용
- 입력 숫자 변수 생성 : readLine() 이용
- 볼,스트라이크 카운트 변수 생성 : 0으로 생성
- 최소,최대 숫자, 입력 갯수 변수 생성 : 1,9,3 으로 생성

랜덤 숫자 생성 기능
-

- 1부터 9까지의 서로 다른 임의의 수로 이루어진 3자리 숫자를 랜덤으로 생성하는 기능이 필요하다.
- pickNumberInRange() 메소드를 사용하여 구현할 수 있다.

사용자 입력 처리 기능
-

- 사용자로부터 1부터 9까지의 서로 다른 3자리 숫자를 입력받아야 한다.
- 중복된 숫자를 입력하거나 3자리를 초과하는 숫자를 입력한 경우 IllegalArgumentException을 발생시켜 게임을 종료해야 한다.
- 사용자 입력은 readLine()을 사용하여 문자열로 받은 후, 이를 List<Integer>로 변환해야 한다.

게임 루프
-

- 사용자가 유효한 숫자를 입력할 때까지 반복되어야 한다.
- 사용자 입력과 랜덤 숫자의 각 자리를 비교하며 볼과 스트라이크를 판단하여 카운트해야 한다.

게임 결과 출력 기능
-

- 볼, 스트라이크 카운트에 따라 적절한 메시지를 출력해야 한다.
- 볼과 스트라이크가 0일 경우 "낫싱"을 출력해야 한다.

게임 재시작 기능
-

- 게임이 종료된 후 사용자에게 게임을 새로 시작할 것인지 물어봐야 한다.
- 사용자 입력이 1이면 게임을 다시 시작하고, 2이면 게임을 종료해야 한다.
- 재시작 또는 종료가 아닌 다른 입력을 받은 경우 IllegalArgumentException을 발생시켜 게임을 종료해야 한다.

예외 처리
-

- 중복된 숫자나 3자리를 초과하는 숫자를 입력한 경우 IllegalArgumentException을 발생시켜야 한다.
- 숫자가 아닌 다른 글자를 입력한 경우에도 IllegalArgumentException을 발생시켜야 한다.

