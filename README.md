# 줌 클론코딩

## 학습하는 것
- P2P, WebRTC를 활용한 유저간 화상 통신, 웹소켓을 활용해 채팅방 생성, 개인 메시지 기능

## HTTP vs WebSockets
- 둘다 protocol
### HTTP
- 모든 서버들이 동작하는 방식 (request -> response 방식)
- 인터넷 전체가 HTTP 기반으로 만들어져있음
- stateless, response 후 backend는 정보를 잃어버리고 request 받을 준비함

### WebSocket
- WebSockbet으로 실시간 chat, notification과 같은 real-time을 만들 수 있음
- WebSocket을 사용해서 연결하고 싶고, 서버가 지원한다면 wss(Secure Web Socket)하면 됨 (wss://nomadcorder.co)
- WebSocket 연결이 일어날 때는 handshake처럼 동작함
  - 브라우저가 서버로 WebSocket request를 보내면, 서버가 받거나 거절함
  - 이렇게 한번 보내고, 받거나 거절이 성립되면 연결은 성립(establish)됨
  - 연결되어있기 때문에, 서버는 정보를 기억함
  - 서버와 클라이언트가 서로 메세지를 주고 받을 수 있음
  - bi-directional(양방향) 연결, 마치 전화통화 같은 것
  - 브라우저 webSocket API를 활용해 작업 예정
  - WebSocket은 어떤 프로그래밍 언어에 국한되어있지 않음
  - WebSocket은 브라우저와 backend 사이에만 발생할 수 있는게 아님


