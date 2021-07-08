

## [OSI 7 layers와 TCP/IP 4 layer](#osi-7-layers와-tcpip-4-layers-답변)
#### 💡 OSI 7 Layer 또는 TCP/IP Layer와 각 계층에 대한 설명을 해주세요.

현대의 웹 모델은 TCP/IP로 넘어오게 되었음
```
Application Layer : TCP/IP 소켓 프로그래밍에서 제공하는 API를 하여 통신가능한 프로그램을 활용할 수 있는 계층

프로토콜 – FTP, HTTP, SSH

Transport Layer : 통신 노드 간의 연결을 제어하고, 신뢰성 있는 데이터 전송을 담당한다.

프로토콜 – TCP, UDP

Internet Layer : 통신 노드 간의 IP패킷을 전송하는 기능과 라우팅 기능을 담당한다.

프로토콜 – IP, ARP, RARP

Network Access Layer : 

OSI 7계층의 물리계층과 데이터 링크 계층에 해당한다.

물리적인 주소로 MAC을 사용한다.

```

#### 💡 OSI 7 Layer 또는 TCP/IP Layer에서 계층화하는 이유가 무엇인가요?

```
1.계층을 분리함으로서 각 계층은 독립적인 역할 수행
2.역할이 분리되면서 문제 발생시 문제의 현상을 보았을 때 어떤 계층인지 파악 가능
```

<del>#### 💡 Encapsulation과 Decapsulation을 서로 비교하며 설명해주세요 </del>

#### 💡 IP 주소 및 MAC 주소는?
```
IP 주소는 네트워크 통신에 있어서 각각의 통신기기(컴퓨터, 노트북, 스마트폰 등)에 할당된 식별번호
MAC 주소는 통신기기의 하드웨어 자체에 부여된 고유한 식별번호
```

#### 💡 IPV4 vs IPV6 을 설명해주세요.

```
- 지연에 민감한 패킷을 구분하는 기본적인 QoS(Quality of Service)
- NAT를 없앰으로써 주소 공간을 32비트에서 128비트로 확장
- 네트워크 레이어 보안 내장(IPsec)
- 손쉬운 네트워크 관리를 위한 무상태 주소 자동 구성
- 처리 오버헤드가 줄어든 개선된 헤더 구조
```

#### 💡 IPv4의 주소 부족현상을 해결하기 위해 현재 어떤 방법을 사용하고 있나요? - 심화

## [TCP와 UDP](#tcp와-udp-답변)
#### 💡 TCP와 UDP의 특징과 차이점을 설명해주세요.

```
TCP
- 연결형 서비스로 가상 회선 방식을 제공한다.
- 3-way handshaking과정을 통해 연결을 설정하고 4-way handshaking을 통해 해제한다.
- 흐름 제어 및 혼잡 제어.
- 높은 신뢰성을 보장한다.
- UDP보다 속도가 느리다.

특징
- 서버소켓은 연결만을 담당한다.
- 연결과정에서 반환된 클라이언트 소켓은 데이터의 송수신에 사용된다형 서비스로 가상 회선 방식을 제공한다.
- 서버와 클라이언트는 1대1로 연결된다.
- 스트림 전송으로 전송 데이터의 크기가 무제한이다.
- 패킷에 대한 응답을 해야하기 때문에(시간 지연, CPU 소모) 성능이 낮다.
- Streaming 서비스에 불리하다.(손실된 경우 재전송 요청을 하므로)

UDP
- 비연결형 서비스로 데이터그램 방식을 제공한다
- 정보를 주고 받을 때 정보를 보내거나 받는다는 신호절차를 거치지 않는다.
- UDP헤더의 CheckSum 필드를 통해 최소한의 오류만 검출한다.
- 신뢰성이 낮다
- TCP보다 속도가 빠르다

특징
- UDP에는 연결 자체가 없어서(connect 함수 불필요) 서버 소켓과 클라이언트 소켓의 구분이 없다.
- 소켓 대신 IP를 기반으로 데이터를 전송한다.
- 서버와 클라이언트는 1대1, 1대N, N대M 등으로 연결될 수 있다.
- 데이터그램(메세지) 단위로 전송되며 그 크기는 65535바이트로, 크기가 초과하면 잘라서 보낸다.
- 흐름제어(flow control)가 없어서 패킷이 제대로 전송되었는지, 오류가 없는지 확인할 수 없다.
- 파일 전송과 같은 신뢰성이 필요한 서비스보다 성능이 중요시 되는 경우에 사용된다.

```

![UDPTCP](./TCPUDP.png)

#### 💡 TCP를 사용하는 대표적인 프로토콜은 무엇인가요?

```
HTTP 통신
```

#### 💡 3-Handshaking과 4-Handshaking의 과정을 설명해주세요. 

```
3-Handshaking
- CLIENT에서 웹 서버로 연결을 최초시도시 먼저 SYN 패킷을 보냅니다.
- SYN 패킷을 보낸 CLIENT는 SYN-SENT 상태가 됩니다.
- SERVER에서 CLOSED는 PORT가 닫혀있는 상태를 뜻하고, 포트가 서비스 가능한 상태인 LISTEN상태로 만들어주어야 합니다.
- LISTEN상태에서 CLIENT부터 SYN패킷을 받으면 이에 대한 응답으로 SYN + ACK 패킷을 CLIENT로 보냅니다.
- SERVER는 CLIENT IP에 대해 포트 SYN-RECEIVED 상태로 전환됩니다.
- SERVER로부터 SYN+ACK 패킷을 받으면, CLIENT는 ESTABLISHED상태로 변하게 되면서 연결을 확인합니다.
- CLIENT는 SERVER로 SYN에 대한 응답으로 ACK패킷을 보냅니다.
- SERVER는 이 ACK 패킷을 받고 해당 CLIENT IP에 대한 포트 ESTABLISHED상태로 전환됩니다.
```
![3hands](./3hands.png)

```
4-Handshaking
1) 클라이언트에서 서버와의 연결 종료를 위해 서버에 FIN 패킷을 보내고 FIN_WAIT1 상태가 됩니다.
2) 서버는 클라이언트로부터 FIN을 받고 응답 패킷 ACK을 보냅니다. 
상태는 CLOSE_WAIT가 됩니다
3) 서버가 통신이 끝나면, 즉 연결을 종료할 준비가 되면 클라이언트에게 FIN패킷을 보내고 LAST_WAIT 상태가 됩니다  
4) 클라이언트는 확인 패킷 ACK을 보내고 TIME_WAIT 상태가 됩니다.

```
![4hands](./4hands.jpeg)


#### 💡 3-way handshaking 과정에서 클라이언트가 서버가 보낸 ACK+SYN을 받지 못하면? - 서버 심화
```
클라이언트에서 특정 시간을 대기해도 전송이 안되는 경우 요청 SYN을 재전송
```

#### 💡 UDP에서 신뢰도를 보장하는 방법을 설명해주세요.
```
발신 수신 IP 및 프로토콜에서 체크섬을 계산
```

## [HTTP와 HTTPS](#http와-https-답변)
#### 💡 HTTP와 HTTPS를 설명해주세요
```
HTTP
HTTP(Hyper Text Transfer Protocol)란 서버/클라이언트 모델을 따라 데이터를 주고 받기 위한 프로토콜이다.

HTTPS
HyperText Transfer Protocol over Secure Socket Layer, HTTP over TLS, HTTP over SSL, HTTP Secure 등으로 불리는 HTTPS는 HTTP에 데이터 암호화가 추가된 프로토콜이다. HTTPS는 HTTP와 다르게 433번 포트를 사용하며, 네트워크 상에서 중간에 제3자가 정보를 볼 수 없도록 공개키 암호화를 지원
```
#### 💡 HTTP의 단점을 설명해주세요
```
HTTP는 암호화가 추가되지 않았기 때문에 보안에 취약한 반면, HTTPS는 안전하게 데이터를 주고받을 수 있다. 하지만 HTTPS를 이용하면 암호화/복호화의 과정이 필요하기 때문에 HTTP보다 속도가 느리다.(오늘날에는 거의 차이를 못느낄 정도이다.) 또한 HTTPS는 인증서를 발급하고 유지하기 위한 추가 비용이 발생하다.

그렇다면 언제 HTTP를 쓰고, 언제 HTTPS를 쓰는 것이 좋겠는가?

개인 정보와 같은 민감한 데이터를 주고 받아야 한다면 HTTPS를 이용해야 하지만, 단순한 정보 조회 등만을 처리하고 있다면 HTTP를 이용하면 된다.
```

#### 💡 HTTP 1.0+와 HTTP1.1와 HTTP2.0 차이점은 무엇인가요?
```
HTTP 1.0
- TCP Connection당 하나의 URL만 fetch하며, 매번 request/response가 끝나면 연결이 끊기므로 필요할 때마다 다시 연결해야하는 단점이 있어 속도가 현저히 느리다.
URL의 크기가 작고 한번에 가져올 수 있는 데이터의 양이 제한되어 있다.


HTTP 1.1
- HTTP의 인터넷에서 impact를 줄이고 cache를 두어 인터넷 프로토콜 수행이 빠르게 될 수 있도록 성능을 향상하고 있다.
- multiple request에 대한 처리가 가능하고 request/response가 파이프라인 방식으로 진행이 가능하다.
- HTTP 1.1의 모든 요청과 응답은 기본적으로 Persistent Connection을 지원
- 필요 없을 경우에만(HTTP 응답 완료 후 TCP 연결을 끊어야하는 경우) Connection 헤더를 사용했다.

- HTTP 1.1에서는 클라이언트와 서버간의 요청과 응답 효율성을 개선하기 위해 HTTP Pipelining이 등장하였다.
```
#### 💡 비대칭키 또는 공개키 암호화 방식은 무엇인가요?
```
A는 공개키(Public key)와 개인키(Private key)를 생성한다.
공개키 암호화: A의 공개키를 이용하여 암호화된 데이터는 A의 개인키로만 복호화가 가능하다.
개인키 암호화: A의 개인키를 이용하여 암호화된 데이터는 A의 공개키로만 복호화가 가능하다.
B는 A의 공개키를 조회하고, A의 공개키를 이용하여 데이터를 암호화한 후 전송한다.
A는 개인키로 암호화된 데이터를 복호화한다.
```

#### 💡 HTTP REQUEST 방식 중 GET과 POST의 차이을 설명해주세요.
```
사용목적 : GET은 서버의 리소스에서 데이터를 요청할 때, POST는 서버의 리소스를 새로 생성하거나 업데이트할 때 사용한다. 

요청에 body 유무 : GET 은 URL 파라미터에 요청하는 데이터를 담아 보내기 때문에 HTTP 메시지에 body가 없다. POST 는 body 에 데이터를 담아 보내기 때문에 당연히 HTTP 메시지에 body가 존재한다.

멱등성 (idempotent) : GET 요청은 멱등이며, POST는 멱등이 아니다.
```

#### 💡 GET, POST를 제외하고 다른 방식들을 설명해주세요.
```
OPTION : 통신과 관련된 선택사항들에 대한 정보를 요구하는 경우
PUT : Request 메시지에 포함되어 있는 data를 지정한 Request-URI로 저장하기 위함
DELETE : 특정 resource를 지우기 위함
TRACE : 최종 destination까지의 Loopback을 테스트하기 위함
```
#### 💡 조회하기 위한 용도 POST가 아닌 GET 방식을 사용하는 이유?  
```
멱등성 때문에
```
#### 💡 현대 웹 에서는 비연결성을 해결방법을 설명해주세요. - 서버 심화
```
쿠키, 세션, 토큰을 사용
```

## [로드밸런서](#로드밸런서-답변) - 서버 개발자만 답변할 것
#### 💡 로드 밸런싱을 설명해주세요.  
#### 💡 L4 로드 밸런싱과 L7 로드 밸런싱에 대해 설명하고, 차이를 말해보세요  
#### 💡 게이트웨이란?  
#### 💡 서버에 트래픽이 주어졌을 때 어떻게 응답속도를 개선할 수 있는가?  
#### 💡 프라이빗 서브넷과 퍼블릭 서브넷의 차이

## 01-2. Web of Network Overview
## [WEB](#web-답변)
#### 💡 url과 uri에 대해 각각 설명해주세요  
#### 💡 브라우저에 "www.google.com" 입력하면 어떤일이 일어날까요?  
#### 💡 RESTful API란 무엇인가요?  
#### 💡 Ajax는 무엇인가요?  
#### 💡 Ajax의 장점과 단점은 무엇인가요? - 웹 심화  
#### 💡 CORS는 무엇인가요?  
#### 💡 CORS preflight는 무엇인가요? - 웹 심화 
#### 💡 소켓이란 무엇인가요?  
#### 💡 DOM과 가상DOM - 웹 심화  
#### 💡 OAuth란 무엇인가요?  
#### 💡 SPA   

## [cookie와 session](#cookie와-session-답변)
#### 💡 cookie와 session에 대해 설명해주세요  
#### 💡 Session 동작 순서를 설명해주세요.  
#### 💡 cookie를 쓰는 이유를 설명해주세요  
#### 💡 세션 인증방식 단점  
#### 💡 토큰 인증방식
#### 💡 JWT   
#### 💡 토큰 인증방식 단점  
#### 💡 쿠키 인증방식 해결방안  

refered by https://github.com/SSAFY-CS-STUDY/