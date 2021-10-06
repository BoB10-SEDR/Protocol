# 스마트 환경에서의 이상행위와 사이버 공격에 대한 모니터링 및 대응 솔루션 제작 (Protocol)

## Protocol 
서버와 에이전트 사이에 주고 받는 데이터 형식 지정
- 언어 : Cpp

## Project Setting
- 정적 라이브러리 생성
    ```
    $ cd Protocol
    $ cmake Src
    $ cmake --build .
    ```
- 라이브러리를 사용할 곳으로 복사
    ```
    $ cd Protocol
    $ cp Build/LinuxRelease/libprotocol.a 목적지
    ```