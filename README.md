# 스마트 환경에서의 이상행위와 사이버 공격에 대한 모니터링 및 대응 솔루션 제작 (Protocol)

## Protocol 
서버와 에이전트 사이에 주고 받는 데이터 형식 지정
- 언어 : Cpp
- 개발환경 : WSL Ubuntu-20.04
- 개발도구 : Visual studio 2019 or Cmake

### Project Setting
- 플랫폼 : ARM 사용(32bit)
- 정적 라이브러리 셋팅
    
  cppcore 등 외부에서 만든 라이브러리를 WSL Ubuntu에 /usr/local/lib로 옮겨야한다.
  
  플랫폼의 환경에 맞는 라이브러리를 선택하여 사용한다.

  cf) visual studio 2019에서 리눅스 정적 라이브러리 연결 관련 오류가 존재한다고 한다.
    ```
    $ cp libcppcore.a /usr/local/lib
    ```

- Visual Studio 2019 빌드 방법
    ```
    # 빌드 결과물
    PATH : Protocol/Build/ARM/libprotocol.a

- Cmake 사용 시 빌드 방법
    ```
    # 빌드
    $ cd Protocol
    $ cmake Src
    $ cmake --build .

    # 빌드 산출물 경로
    Path :  Protocol/Build/LinuxRelease/libprotocol.a
    ```

