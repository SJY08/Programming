## Node.js 란 ?

> Node.js는 Chrome V8 JavaScript 엔진으로 빌드된 JavaScript 런타임(=환경)

**Node js는 확장성 있는 네트워크 애플리케이션(특히 서버사이드) 개발에 사용되는 소프트웨어 플랫폼**

-   내장 http 서버 라이브러리를 포함하고 있어 웹 서버에서 별도의 소프트웨어 없이 동작이 가능
-   **논 블로킹(Non-blocking) I/O**와 **단일 스레드 이벤트 루프**를 통한 **높은 처리 성능**

## Non-blocking I/O란 ?

-   **Non-blocking I/O란 ?** 한 프로세스가 IO 작업을 호출했을 때, IO 작업이 완료될 때 까지 작업을 중단하지 않고 IO 호출에 대해 **즉시 리턴**, 해당 프로세스에 이어 **다음 IO 작업을 수행할 수 있게 하는 방식**

## 이벤트 루프란 ?

-   **이벤트 루프란 ?** 브라우저의 동작 타이밍을 제어하는 관리자

-   라우저 내부의 Call Stack, Callback Queue, Web APIs 등의 요소들을 모니터링하면서 비동기적으로 실행되는 작업들을 관리하고, 이를 순서대로 처리하여 프로그램의 실행 흐름을 제어

동작 과정
![image](https://blog.kakaocdn.net/dn/pedOg/btrzvTs6JnP/IC6ZFXYWLrHDDubDe3Equ0/img.png)
