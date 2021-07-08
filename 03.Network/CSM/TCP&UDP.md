## TCP와 UDP

#### 💡TCP와 UDP의 특징과 차이점을 설명해주세요.

- TCP는 연결형 서비스이고, 데이터의 흐름 제어나 혼잡 제어 기능을 하기 신뢰성을 보장합니다. 하지만 UDP보다는속도가 느리게 됩니다. (이런 기능들은 CPU를 사용하기 때문에 속도에 영향을 주는 것)

  UDP는 비연결형 서비스이고, 정보를 주고 받을 때, 정보를 보내거나 받는다는 신호 절차를 거치지 않기 때문에 신뢰성이 낮으나, TCP보다 속도가 빠릅니다.

  따라서 TCP는 연속성보다 신뢰성 있는 전송이 중요할 때(ex. 파일 전송) 사용하고, UDP는 신뢰성보다 연속성이 중요한 서비스 (ex. 실시간 스트리밍 서비스)에 사용됩니다.

<br>

#### 💡 TCP를 사용하는 대표적인 프로토콜은 무엇인가요?

- TCP는 주로 대부분의 웹 HTTP 통신, 이메일, 파일 전송에 사용됩니다.

<br>

#### 💡 3-Handshaking과 4-Handshaking의 과정을 설명해주세요. 

- 3-way handshaking은 3단계로 나눠집니다

  먼저, A 클라이언트는 B 서버에 접속을 요청하는 SYN 패킷을 보내고, SYN/ACK 응답을 기다리는 SYN_SENT 상태가 됩니다.

  B 서버가 SYN 요청을 받으면, A 클라이언트에게 요청을 수락한다는 ACK와 SYN flag가 설정된 패킷을 발송하고, A가 다시 ACK로 응답하기를 기다립니다. 이 때, B 서버는 SYN_RECEIVED 상태가 됩니다.

  마지막으로, A 클라이언트는 B에게 ACK을 보내고 이후부터는 연결이 이뤄지고 데이터가 오가게 됩니다. 이 때, B 서버의 상태가 ESTABLISHED가 됩니다.

  3-way handshaking은 TCP의 연결을 초기화할 때 사용합니다.

- 반면에 4-way handshaking은 세션을 종료하기 위해 수행하는 절차이고, 4단계로 이뤄집니다.

  먼저, 클라이언트가 연결을 종료하겠다는 FIN 플래그를 전송합니다.

  그러면 서버는 일단 확인 메세지를 보내고, 자신의 통신이 끝날 때까지 기다리는데 이 상태가 TIME_WAIT 상태입니다.

  서버가 통신이 끝났으면, 연결이 종료되었다고 클라이언트에게 FIN 플래그를 전송합니다.

  마지막으로, 클라이언트는 확인했다는 메세지를 서버에게 보내게 됩니다.

<br>

#### 💡 3-way handshaking 과정에서 클라이언트가 서버가 보낸 ACK+SYN을 받지 못하면? - 서버 심화

- 클라이언트는 서버에게 SYN을 보내고 시간을 잽니다. Timeout이 되기 전까지 서버에게 ACK+SYN을 받지 못하면 클라이언트는 다시 SYN을 보내고 대기합니다.


<br>

#### 💡 UDP에서 신뢰도를 보장하는 방법을 설명해주세요.

- UDP의 특성을 살리면서 TCP처럼 신뢰할 수 있는 데이터를 만드는 Reliable UDP를 사용합니다.

<br>

<br>

## 🏃🏻‍♀️ 정리





<br>

---

**[참고]**

[TCP와 UDP의 특징과 차이](https://mangkyu.tistory.com/15)

[TCP 3 Way-Handshake & 4 Way-Handshake](https://mindnet.tistory.com/entry/%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC-%EC%89%BD%EA%B2%8C-%EC%9D%B4%ED%95%B4%ED%95%98%EA%B8%B0-22%ED%8E%B8-TCP-3-WayHandshake-4-WayHandshake)

[Reliable UDP](http://blog2928.kc39.net/13263)