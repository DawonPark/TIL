# 웹의 동작 방식

## 클라이언트와 서버
![서버와 클라이언트 상호작용](https://mdn.mozillademos.org/files/8973/Client-server.jpg)
- 웹에 연결된 컴퓨터는 **클라이언트**와 **서버**라고 한다.
- 클라이언트는 일반적으로 웹 사용자의 인터넷이 연결된 장치들 핸드폰이나 컴퓨터들과 이 장치들로 이용가능한 웹에 접근 하는 소프트웨어
- 서버는 웹페이지, 사이트, 앱을 저장하는 컴퓨터이다. 클라이언트의 장비가 접근을 원할 때 서버로 부터 웹 브라우저에 보여지기 위한 웹페이지 사본이 다운로드 된다.

## 클라이언트와 서버의 동작

### 기본지식
- **인터넷 연결** : 웹에서 데이터를 보내고 받을 수 있다.
- **TCP/IP** : Transmission Control Protocol(전송 제어 규약)과 Internet Protocol(인터넷 규약)은 데이터가 어떻게 웹에서 전송하는지 정의하는 통신 규약
- **DNS** : Domain Name System Servers(도메인 이름 시스템 서버)는 웹사이트를 위한 주소록과 같다. 브라우저에 웹 주소를 입력할 때, 브라우저는 그 웹사이트를 검색하기 전에 DNS를 살펴보고 HTTP 메시지를 올바른 장소로 전송하기 위해 웹사이트가 있는 서버가 어떤 것인지 찾아야한다.
- **컴포넌트 파일**
  - **코드 파일** : HTML,CSS, JavaScript
  - **자원** : 이미지, 음악, 비디오, 단어 문서, 웹사이트를 만드는 모든 다른 것들을 위한 공동적 이름

### 동작
- 브라우저는 DNS 서버로 가서 웹사이트가 있는 서버의 진짜 주소를 찾는다.
- 브라우저는 서버에게 웹사이트 사본을 클라이언트에게 보내달라는 HTTP 요청 메세지를 서버로 전송 이 메세지와 모든 데이터는 TCP/IP 연결을 통해 전송된다.
- 메세지를 받은 서버는 클라이언트의 요청을 승인하고 "200 OK" 메세지를 클라이언트에게 전송 후 서버는 웹사이트의 파일들을 데이터 패킷이라 불리는 작은 일련의 덩어리들로 브라우저에 전송 시작한다.
- 브라우저는 이 패킷을 완전한 웹사이트로 조립하고 보여준다.

참고 : https://developer.mozilla.org/ko/docs/Learn/Getting_started_with_the_web/How_the_Web_works