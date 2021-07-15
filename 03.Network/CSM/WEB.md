## WEB

#### 💡 url과 uri에 대해 각각 설명해주세요.

- URI는 어떤 자원을 식별하기 위한 문자열의 구성이고, URL과 URN의 상위 개념으로서 이들을 포함하고 있습니다.

  URL은 인터넷 상에서 어떤 자원을 식별할 때 자원의 위치를 활용하여 특정 자원을 식별합니다.

<br>

#### 💡 브라우저에 "www.google.com" 입력하면 어떤일이 일어날까요? ⭐️

- 브라우저는 DNS 서버로 가서 도메인을 확인하고, 웹 사이트가 있는 서버의 IP 주소를 찾습니다. 이후, 서버에게 웹사이트의 사본을 클라이언트에게 보내달라는 HTTP 요청 메세지를 서버로 전송합니다. 서버는 클라이언트의 요청을 승인하고, 웹 사이트의 정보를 패킷으로 묶어서 브라우저로 보냅니다. 브라우저는 이 패킷들을 활용하여 웹 사이트로 만들어 사용자에게 보여줍니다.

<br>

#### 💡 RESTful API란 무엇인가요?  

- RESTful API는 REST API 설계 가이드를 따라 API를 만드는 것입니다.

  REST란 어떤 자원에 대해 CRUD(Create, Read, Update, Delete) 연산을 수행하기 위해 URI(Resource)로 요청을 보내는 것으로, Get, Post 등의 방식(Method)를 사용해 요청을 보내며, 요청을 위한 자원은 특정한 형태로 표현됩니다. 그리고 이러한 REST 기반의 API를 웹으로 구현한 것이 RESTful API입니다.


<br>

#### 💡 Ajax는 무엇인가요?

- Ajax는 JavaScript 라이브러리 중 하나이며, 브라우저가 가지고 있는 XMLHttpRequest 객체를 이용해서 전체 페이지를 새로 고치지 않고도 페이지의 일부만을 위한 데이터를 로드하는 기법입니다.

  쉽게 말해, 자바스크립트를 통해 서버에 데이터를 요청하는 것입니다. (비동기 방식)

<br>

#### 💡 Ajax의 장점과 단점은 무엇인가요? - 웹 심화

- 장점은 서버의 처리가 완료될 때까지 기다리지 않고 처리가 가능 (비동기 방식)하다는 점이고, 단점은 연속으로 데이터를 요청하면 서버 부하가 증가할 수 있다는 점입니다.

<br>

#### 💡 CORS는 무엇인가요? ⭐️

- CORS란 현재 IP가 아닌 다른 IP로 리소스를 요청하는 구조입니다. 추가 HTTP헤더를 사용해 한 출처에서 실행 중인 웹 어플리케이션이 다른 출처의 선택한 자원에 접근할 수 있는 권한을 부여하도록 브라우저에 알려주는 체제입니다.

  CORS는 기본적으로 요청 헤더의 Origin 필드에 요청을 보내는 출처를 담아 전송합니다. 서버는 요청에 대한 응답을 하는데, 응답 헤더 (response header)에 Access-Control-Allow-Origin이라는 값에 '이 리소스를 접근하는 것이 허용된 출처'를 내려줍니다. 이후, 응답을 받은 브라우저는 자신이 보냈던 요청의 Origin과 서버가 보내준 응답의 Access-Control-Allow-Origin을 비교해본 후, 이 응답이 유효한 응답인지 아닌지를 결정합니다.

<br>

#### 💡 CORS preflight는 무엇인가요? - 웹 심화 

- 

<br>

#### 💡 소켓이란 무엇인가요?  

- 소켓은 서버와 클라이언트가 특정 Port를 통해 연결을 성립하고 있어, 실시간으로 양방향 통신을 하는 방식입니다.

<br>

#### 💡 DOM과 가상DOM - 웹 심화  

- 

<br>

#### 💡 OAuth란 무엇인가요?  

- OAuth는 다른 응용프로그램의 사용자 계정에 대한 제한된 액세스를 요청할 수 있도록 하는 권한 부여 프레임워크입니다. 쉽게 말해서 다른 서비스의 회원 정보를 안전하게 사용하기 위한 방법입니다.

<br>

#### 💡 SPA

- SPA는 단일 페이지로 구성된 웹 어플리케이션을 말합니다. SPA는 화면 이동시에 필요한 데이터를 서버사이드에서 HTML로 전달받지 않고, 필요한 데이터만 서버로부터 JSON으로 전달받아 동적으로 렌더링합니다.

  기존에는 사용자가 새로운 페이지로 이동할 때마다 새로운 HTML을 받아와 페이지를 로드해 보여주었다면, 현재의 페이지를 동적으로 다시 작성하는 방식입니다. (ex. 페이스북, 에어비앤비, 트위터, 넷플릭스 등에서 사용)

<br>

<br>

## 🏃🏻‍♀️ 정리





<br>

---

**[참고]**

[URL과 URI](https://velog.io/@jch9537/URI-URL)

[URL과 URI, URN](https://juyeop.tistory.com/48)

[DNS](https://velog.io/@doomchit_3/Internet-DNS-%EC%9E%91%EB%8F%99%EC%9B%90%EB%A6%AC-IMBETPY)

[웹 사이트 접속 방식](https://coding-factory.tistory.com/719)

[REST API](https://velog.io/@taeha7b/api-restapi-restfulapi)

[RESTful API](https://mangkyu.tistory.com/46)

[AJAX](https://velog.io/@surim014/AJAX%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%B8%EA%B0%80)

[CORS](https://velog.io/@pilyeooong/CORS%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%B8%EA%B0%80)

[소켓](https://qlyh8.tistory.com/86)

[HTTP 통신 방식과 소켓 통신 방식의 차이](https://mangkyu.tistory.com/48)

[OAuth](https://velog.io/@undefcat/OAuth-2.0-%EA%B0%84%EB%8B%A8%EC%A0%95%EB%A6%AC)

[SPA](https://velog.io/@josworks27/SPA-%EA%B0%9C%EB%85%90)