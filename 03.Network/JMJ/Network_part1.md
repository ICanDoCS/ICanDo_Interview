

## [OSI 7 layers์ TCP/IP 4 layer](#osi-7-layers์-tcpip-4-layers-๋ต๋ณ)
#### ๐ก OSI 7 Layer ๋๋ TCP/IP Layer์ ๊ฐ ๊ณ์ธต์ ๋ํ ์ค๋ช์ ํด์ฃผ์ธ์.

![image-20210708221219552](image/1.png)

##### 1) ๋ฌผ๋ฆฌ(Physical)

> ๋ฆฌํผํฐ, ์ผ์ด๋ธ, ํ๋ธ ๋ฑ

๋จ์ง ๋ฐ์ดํฐ ์ ๊ธฐ์ ์ธ ์ ํธ๋ก ๋ณํํด์ ์ฃผ๊ณ ๋ฐ๋ ๊ธฐ๋ฅ์ ์งํํ๋ ๊ณต๊ฐ

์ฆ, ๋ฐ์ดํฐ๋ฅผ ์ ์กํ๋ ์ญํ ๋ง ์งํํ๋ค.



##### 2) ๋ฐ์ดํฐ ๋งํฌ(Data Link)

> ๋ธ๋ฆฟ์ง, ์ค์์น ๋ฑ

๋ฌผ๋ฆฌ ๊ณ์ธต์ผ๋ก ์ก์์ ๋๋ ์ ๋ณด๋ฅผ ๊ด๋ฆฌํ์ฌ ์์ ํ๊ฒ ์ ๋ฌ๋๋๋ก ๋์์ฃผ๋ ์ญํ 

Mac ์ฃผ์๋ฅผ ํตํด ํต์ ํ๋ค. ํ๋ ์์ Mac ์ฃผ์๋ฅผ ๋ถ์ฌํ๊ณ  ์๋ฌ๊ฒ์ถ, ์ฌ์ ์ก, ํ๋ฆ์ ์ด๋ฅผ ์งํํ๋ค.



##### 3) ๋คํธ์ํฌ(Network)

> ๋ผ์ฐํฐ, IP

๋ฐ์ดํฐ๋ฅผ ๋ชฉ์ ์ง๊น์ง ๊ฐ์ฅ ์์ ํ๊ณ  ๋น ๋ฅด๊ฒ ์ ๋ฌํ๋ ๊ธฐ๋ฅ์ ๋ด๋นํ๋ค.

๋ผ์ฐํฐ๋ฅผ ํตํด ์ด๋ํ  ๊ฒฝ๋ก๋ฅผ ์ ํํ์ฌ IP ์ฃผ์๋ฅผ ์ง์ ํ๊ณ , ํด๋น ๊ฒฝ๋ก์ ๋ฐ๋ผ ํจํท์ ์ ๋ฌํด์ค๋ค.

๋ผ์ฐํ, ํ๋ฆ ์ ์ด, ์ค๋ฅ ์ ์ด, ์ธ๊ทธ๋จผํ์ด์ ๋ฑ์ ์ํํ๋ค.



##### 4) ์ ์ก(Transport)

> TCP, UDP

TCP์ UDP ํ๋กํ ์ฝ์ ํตํด ํต์ ์ ํ์ฑํํ๋ค. ํฌํธ๋ฅผ ์ด์ด๋๊ณ , ํ๋ก๊ทธ๋จ๋ค์ด ์ ์ก์ ํ  ์ ์๋๋ก ์ ๊ณตํด์ค๋ค.

\- TCP : ์ ๋ขฐ์ฑ, ์ฐ๊ฒฐ์งํฅ์ 

\- UDP : ๋น์ ๋ขฐ์ฑ, ๋น์ฐ๊ฒฐ์ฑ, ์ค์๊ฐ



##### 5) ์ธ์(Session)

> API, Socket

๋ฐ์ดํฐ๊ฐ ํต์ ํ๊ธฐ ์ํ ๋ผ๋ฆฌ์  ์ฐ๊ฒฐ์ ๋ด๋นํ๋ค. TCP/IP ์ธ์์ ๋ง๋ค๊ณ  ์์ ๋ ์ฑ์์ ์ง๋๊ณ  ์๋ค.



##### 6) ํํ(Presentation)

> JPEG, MPEG ๋ฑ

๋ฐ์ดํฐ ํํ์ ๋ํ ๋๋ฆฝ์ฑ์ ์ ๊ณตํ๊ณ  ์ํธํํ๋ ์ญํ ์ ๋ด๋นํ๋ค.

ํ์ผ ์ธ์ฝ๋ฉ, ๋ช๋ น์ด๋ฅผ ํฌ์ฅ, ์์ถ, ์ํธํํ๋ค.



##### 7) ์์ฉ(Application)

> HTTP, FTP, DNS ๋ฑ

์ต์ข ๋ชฉ์ ์ง๋ก, ์์ฉ ํ๋ก์ธ์ค์ ์ง์  ๊ด๊ณํ์ฌ ์ผ๋ฐ์ ์ธ ์์ฉ ์๋น์ค๋ฅผ ์ํํ๋ค.

์ฌ์ฉ์ ์ธํฐํ์ด์ค, ์ ์์ฐํธ, ๋ฐ์ดํฐ๋ฒ ์ด์ค ๊ด๋ฆฌ ๋ฑ์ ์๋น์ค๋ฅผ ์ ๊ณตํ๋ค.



#### ๐ก OSI 7 Layer ๋๋ TCP/IP Layer์์ ๊ณ์ธตํํ๋ ์ด์ ๊ฐ ๋ฌด์์ธ๊ฐ์?

- ์์คํ ๊ฐ์ ํต์ ์ ๊ฐ๋ฐฉํ๊ธฐ ์ํด์ (OSI 7๊ณ์ธต์ด ์๊ธฐ๊ธฐ ์ด์ ์๋ ํ์ค์ด ์กด์ฌํ์ง ์์ ๊ฐ์๊ฐ์์ผ๋ก ๊ฐ๋ฐ์ ํ๊ธฐ ๋๋ฌธ์ ๋ฐ์ดํฐ ์ ์ก์ด ์ด๋ ค์ ์)

- ํต์ ์ด ์ผ์ด๋๋ ๊ณผ์ ์ ๋จ๊ณ๋ณ๋ก ์ ์ ์๊ณ , ํน์ ํ ๊ณณ์ ์ด์์ด ์๊ธฐ๋ฉด ๊ทธ ๋จ๊ณ๋ง ์์ ํ  ์ ์๊ธฐ ๋๋ฌธ์ด๋ค.

  

#### ๐ก Encapsulation๊ณผ Decapsulation์ ์๋ก ๋น๊ตํ๋ฉฐ ์ค๋ชํด์ฃผ์ธ์

> ์บก์ํ๋ ๋ฐ์ดํฐ๊ฐ ์ถ๊ฐ๋จ, ์ญ ์บก์ํ๋ ์ ๋ณด๋ฅผ ์ ๊ฑฐํจ

- **Encapsulation** (์บก์ํ)

  - ์์ ๊ณ์ธต์์ ํ์ ๊ณ์ธต์ผ๋ก ์ด๋ํ๋ฉด์ ๊ฐ ๊ณ์ธต์ ๊ธฐ๋ฅ๋ค์ ํค๋์ ๋ด์์ ํฉ์น๋ ๋ฐฉ์
  - ํต์ ํ  ๋, ์ ์ด์ ์ฃผ์ ์ ๋ณด๋ฅผ ๊ฐ์ง๊ณ  ์๋ ํค๋๊ฐ ๊ณ์ธต์ ๋ด๋ ค๊ฐ๋ฉฐ ๋ฐ์ดํฐ์ ์ถ๊ฐ๋๋ ๊ฒ 

- **Decapsulation** (์ญ ์บก์ํ)

  - ์์ ํ ๋ฐ์ดํฐ๋ฅผ ํ์ ๊ณ์ธต์์ ์์ ๊ณ์ธต์ผ๋ก ์ฌ๋ผ๊ฐ ๋, ๊ฐ ๊ณ์ธต๋ค์ ํค๋๋ฅผ ํ๋ฉด์ ์ฌ๋ผ๊ฐ๋ ๋ฐฉ์

  - ์ถ๊ฐ ์ ๋ณด๋ฅผ ์ ๊ฑฐํ๊ณ  ์์ ์ง์ ๊ณ์ธต๊น์ง์ ์์ฉ๋ฐ์ดํฐ๋ง ๋ณด๋ด๋ ๊ฒ

    

#### ๐ก IP ์ฃผ์ ๋ฐ MAC ์ฃผ์๋?

> ๊ณตํต์ , ๋คํธ์ํฌ ํต์ ์์ ํต์ ๊ธฐ๊ธฐ์ ์๋ณ๋ฒํธ๋ฅผ ๋ํ๋ด๋ ๊ฒ

- MAC ์ฃผ์

  - ๋ฐ์ดํฐ ๋งํฌ ๊ณ์ธต(2๊ณ์ธต)์์ ์ฌ์ฉํ๋ ๋คํธ์ํฌ ์ธํฐํ์ด์ค์ ํ ๋น๋ ๊ณ ์  ์๋ณ ์ฃผ์

  - ๋ฌผ๋ฆฌ ์ฃผ์๋ ํ๋์จ์ด ์ฃผ์๋ผ๊ณ ๋ ๋ถ๋ฆฐ๋ค.

    ex) D1:F2:FK:CC:12:34

- IP ์ฃผ์

  - ํธ์คํธ๋ ๋ผ์ฐํฐ ์ฅ๋น์ ์ธํฐํ์ด์ค์ ํ ๋น๋ 32bit์ ์ฃผ์(IPv4๊ธฐ์ค, IPv6๋ 128bit)

  - ์ด ์ฃผ์๋ฅผ ํตํด์, ์ฅ์น๋ค์ด ์๋ก๋ฅผ ์ธ์ํ๊ณ  ํต์ ํ  ์ ์์ต๋๋ค.

    ex) 192.168.107.11

    

#### ๐ก IPV4 vs IPV6 ์ ์ค๋ชํด์ฃผ์ธ์.

| ๊ตฌ๋ถ              | IPv4                                 | IPv6                                                         |
| ----------------- | ------------------------------------ | ------------------------------------------------------------ |
| ์ฃผ์๊ธธ์ด          | 32bit                                | 128bit                                                       |
| ํ์ ๋ฐฉ๋ฒ         | 8๋นํธ์ฉ 4๋ถ๋ถ 10์ง์ ํ์            | 16๋นํธ 8๋ถ๋ถ 16์ง์๋ก ํ์                                   |
| ์ฃผ์ ๊ฐ์         | ์ฝ 43์ต๊ฐ                            | 2^128๊ฐ                                                      |
| ์ฃผ์ํ ๋น ๋ฐฉ์     | A,B,C,D ๋ฑ์ ํด๋์ค ๋จ์ ๋น์์ฐจ ํ ๋น | ๋คํธ์ํฌ ๊ท๋ชจ, ๋จ๋ง๊ธฐ์์ ๋ฐ๋ผ ์์ฐจ ํ ๋น                     |
| ๋ธ๋กํธ์บ์คํธ ์ฃผ์ | ์์                                 | ์์, ๋์  ๋ก์ปฌ๋ฒ์ ๋ด์์ ๋ชจ๋  ๋ธ๋์ ๋ํ ๋ฉํฐ์บ์คํธ ์ฃผ์ ์ฌ์ฉ |
| ํค๋ ํฌ๊ธฐ         | ๊ฐ๋ณ                                 | ๊ณ ์                                                          |
| ๋ณด์              | IPSec ํ๋กํ ์ฝ ๋ณ๋ ์ค์น             | IPSec ์์ฒด ์ง์(๋ณด์์ฑ ๊ฐํ)                                 |
| ์๋น์ค ํ์ง       | ์ ํ์  ํ์ง ๋ณด์ฅ                     | ํ์ฅ๋ ํ์ง ๋ณด์ฅ(ํธ๋ํฝ ํจ๊ณผ์ ์ผ๋ก ๋ถ๋ฅ-ํ๋ก์ฐ ๋ ์ด๋ธ(Flow Label) ํ๋ ์ด์ฉ) |
| QoS ์ ๊ณต          | ๋ฏธํก                                 | ์ ๊ณต                                                         |



#### ๐ก IPv4์ ์ฃผ์ ๋ถ์กฑํ์์ ํด๊ฒฐํ๊ธฐ ์ํด ํ์ฌ ์ด๋ค ๋ฐฉ๋ฒ์ ์ฌ์ฉํ๊ณ  ์๋์? - ์ฌํ

- **IPv6**

  - ํ์ฌ ์ธํฐ๋ท ํ๋กํ ์ฝ์ธ IPv4์ ํ๊ณ์ธ ์ฃผ์ ํํ์ ์ ์ฝ์ผ๋ก ์ธํ **์ฃผ์๊ณ ๊ฐ** ๋ฐ **๋ฉํฐ๋ฏธ๋์ด ์๋น์ค ๋์ ๋ฏธ์ฝ** ๋ฑ์ ๊ณ ๋ คํ์ฌ ์๊ธด ์ฐจ์ธ๋ ์ธํฐ๋ท ํ๋กํ ์ฝ

    

## [TCP์ UDP](#tcp์-udp-๋ต๋ณ)
#### ๐ก TCP์ UDP์ ํน์ง๊ณผ ์ฐจ์ด์ ์ ์ค๋ชํด์ฃผ์ธ์.

> ๋คํธ์ํฌ ๊ณ์ธต ์ค **์ ์ก ๊ณ์ธต**์์ ์ฌ์ฉํ๋ ํ๋กํ ์ฝ

- TCP(Transmission Control Protocol)
  - ์ธํฐ๋ท ์์์ ๋ฐ์ดํฐ๋ฅผ ๋ฉ์ธ์ง์ ํํ(**์ธ๊ทธ๋จผํธ** ๋ผ๋ ๋ธ๋ก ๋จ์)๋ก ๋ณด๋ด๊ธฐ ์ํด IP์ ํจ๊ป ์ฌ์ฉํ๋ ํ๋กํ ์ฝ์ด๋ค.

  - TCP์ IP๋ฅผ ํจ๊ป ์ฌ์ฉํ๋๋ฐ, IP๊ฐ ๋ฐ์ดํฐ์ ๋ฐฐ๋ฌ์ ์ฒ๋ฆฌํ๋ค๋ฉด TCP๋ ํจํท์ ์ถ์  ๋ฐ ๊ด๋ฆฌํ๋ค.

  - ์ฐ๊ฒฐํ ์๋น์ค๋ก ๊ฐ์ ํ์  ๋ฐฉ์์ ์ ๊ณตํ๋ค.

    - **3-way handshaking๊ณผ์ ์ ํตํด ์ฐ๊ฒฐ์ ์ค์ ํ๊ณ , 4-way handshaking์ ํตํด ์ฐ๊ฒฐ์ ํด์ ํ๋ค.**

  - ํ๋ฆ์ ์ด ๋ฐ ํผ์ก์ ์ด๋ฅผ ์ ๊ณตํ๋ค.

    - ํ๋ฆ์ ์ด
      - ๋ฐ์ดํฐ๋ฅผ ์ก์ ํ๋ ๊ณณ๊ณผ ์์ ํ๋ ๊ณณ์ ๋ฐ์ดํฐ ์ฒ๋ฆฌ ์๋๋ฅผ ์กฐ์ ํ์ฌ ์์ ์์ ๋ฒํผ ์ค๋ฒํ๋ก์ฐ๋ฅผ ๋ฐฉ์งํ๋ ๊ฒ
      - ์ก์ ํ๋ ๊ณณ์์ ๊ฐ๋น์ด ์๋๊ฒ ๋ง์ ๋ฐ์ดํฐ๋ฅผ ๋น ๋ฅด๊ฒ ๋ณด๋ด ์์ ํ๋ ๊ณณ์์ ๋ฌธ์ ๊ฐ ์ผ์ด๋๋ ๊ฒ์ ๋ง๋๋ค.
    - ํผ์ก์ ์ด
      - ๋คํธ์ํฌ ๋ด์ ํจํท ์๊ฐ ๋์น๊ฒ ์ฆ๊ฐํ์ง ์๋๋ก ๋ฐฉ์งํ๋ ๊ฒ
      - ์ ๋ณด์ ์ํต๋์ด ๊ณผ๋คํ๋ฉด ํจํท์ ์กฐ๊ธ๋ง ์ ์กํ์ฌ ํผ์ก ๋ถ๊ดด ํ์์ด ์ผ์ด๋๋ ๊ฒ์ ๋ง๋๋ค.

  - **๋์ ์ ๋ขฐ์ฑ์ ๋ณด์ฅํ๋ค.**

  - **UDP๋ณด๋ค ์๋๊ฐ ๋๋ฆฌ๋ค.**

  - ์ ์ด์ค(Full-Duplex), ์ ๋์ (Point to Point) ๋ฐฉ์์ด๋ค.

    - ์ ์ด์ค
      - ์ ์ก์ด ์๋ฐฉํฅ์ผ๋ก ๋์์ ์ผ์ด๋  ์ ์๋ค.
    - ์ ๋์ 
      - ๊ฐ ์ฐ๊ฒฐ์ด ์ ํํ 2๊ฐ์ ์ข๋จ์ ์ ๊ฐ์ง๊ณ  ์๋ค.
    - ๋ฉํฐ์บ์คํ์ด๋ ๋ธ๋ก๋์บ์คํ์ ์ง์ํ์ง ์๋๋ค.

  - ์ฐ์์ฑ๋ณด๋ค ์ ๋ขฐ์ฑ์๋ ์ ์ก์ด ์ค์ํ  ๋์ ์ฌ์ฉ๋๋ค. **HTTPํต์ ์ ์ฌ์ฉ๋๋ค.**

    

- UDP(User Datagram Protocol)
  - ๋ฐ์ดํฐ๋ฅผ **๋ฐ์ดํฐ๊ทธ๋จ** ๋จ์๋ก ์ฒ๋ฆฌํ๋ ํ๋กํ ์ฝ์ด๋ค.

  - ๋น์ฐ๊ฒฐํ ์๋น์ค๋ก ๋ฐ์ดํฐ๊ทธ๋จ ๋ฐฉ์์ ์ ๊ณตํ๋ค.

    - ์ฐ๊ฒฐ์ ์ํด ํ ๋น๋๋ ๋ผ๋ฆฌ์ ์ธ ๊ฒฝ๋ก๊ฐ ์๋ค.
    - ๊ทธ๋ ๊ธฐ ๋๋ฌธ์ ๊ฐ๊ฐ์ ํจํท์ ๋ค๋ฅธ ๊ฒฝ๋ก๋ก ์ ์ก๋๊ณ , ๊ฐ๊ฐ์ ํจํท์ ๋๋ฆฝ์ ์ธ ๊ด๊ณ๋ฅผ ์ง๋๊ฒ ๋๋ค.
    - ์ด๋ ๊ฒ ๋ฐ์ดํฐ๋ฅผ ์๋ก ๋ค๋ฅธ ๊ฒฝ๋ก๋ก ๋๋ฆฝ์ ์ผ๋ก ์ฒ๋ฆฌํ๋ค.

  - ์ ๋ณด๋ฅผ ์ฃผ๊ณ  ๋ฐ์ ๋ ์ ๋ณด๋ฅผ ๋ณด๋ด๊ฑฐ๋ ๋ฐ๋๋ค๋ ์ ํธ์ ์ฐจ๋ฅผ ๊ฑฐ์น์ง ์๋๋ค.

  - UDPํค๋์ CheckSum ํ๋๋ฅผ ํตํด ์ต์ํ์ ์ค๋ฅ๋ง ๊ฒ์ถํ๋ค.

  - ์ ๋ขฐ์ฑ์ด ๋ฎ๋ค.

  - TCP๋ณด๋ค ์๋๊ฐ ๋น ๋ฅด๋ค.

  - ์ ๋ขฐ์ฑ๋ณด๋ค๋ ์ฐ์์ฑ์ด ์ค์ํ ์๋น์ค, ์๋ฅผ ๋ค๋ฉด **์ค์๊ฐ ์๋น์ค(streaming)์ ์ฌ์ฉ**๋๋ค.

    

#### ๐ก TCP๋ฅผ ์ฌ์ฉํ๋ ๋ํ์ ์ธ ํ๋กํ ์ฝ์ ๋ฌด์์ธ๊ฐ์?

- HTTP ํต์ 



#### ๐ก 3-Handshaking๊ณผ 4-Handshaking์ ๊ณผ์ ์ ์ค๋ชํด์ฃผ์ธ์. 

- **3 way handshake - ์ฐ๊ฒฐ ์ฑ๋ฆฝ**

> TCP๋ ์ ํํ ์ ์ก์ ๋ณด์ฅํด์ผ ํ๋ค. 
>
> ๋ฐ๋ผ์ ํต์ ํ๊ธฐ์ ์์, ๋ผ๋ฆฌ์ ์ธ ์ ์์ ์ฑ๋ฆฝํ๊ธฐ ์ํด 3 way handshake ๊ณผ์ ์ ์งํํ๋ค.

[![img](https://camo.githubusercontent.com/4acea6af95884347810f057d00c6c4643a56d4a7dbbdf49740745560cd45cc1f/68747470733a2f2f6d656469612e6765656b73666f726765656b732e6f72672f77702d636f6e74656e742f75706c6f6164732f5443502d636f6e6e656374696f6e2d312e706e67)](https://camo.githubusercontent.com/4acea6af95884347810f057d00c6c4643a56d4a7dbbdf49740745560cd45cc1f/68747470733a2f2f6d656469612e6765656b73666f726765656b732e6f72672f77702d636f6e74656e742f75706c6f6164732f5443502d636f6e6e656374696f6e2d312e706e67)

1. ํด๋ผ์ด์ธํธ๊ฐ ์๋ฒ์๊ฒ SYN ํจํท์ ๋ณด๋ (sequence : x)
2. ์๋ฒ๊ฐ SYN(x)์ ๋ฐ๊ณ , ํด๋ผ์ด์ธํธ๋ก ๋ฐ์๋ค๋ ์ ํธ์ธ ACK์ SYN ํจํท์ ๋ณด๋ (sequence : y, ACK : x + 1)
3. ํด๋ผ์ด์ธํธ๋ ์๋ฒ์ ์๋ต์ ACK(x+1)์ SYN(y) ํจํท์ ๋ฐ๊ณ , ACK(y+1)๋ฅผ ์๋ฒ๋ก ๋ณด๋

์ด๋ ๊ฒ 3๋ฒ์ ํต์ ์ด ์๋ฃ๋๋ฉด ์ฐ๊ฒฐ์ด ์ฑ๋ฆฝ๋๋ค. (3๋ฒ์ด๋ผ 3 way handshake์ธ ๊ฒ)



- **4 way handshake - ์ฐ๊ฒฐ ํด์ **

> ์ฐ๊ฒฐ ์ฑ๋ฆฝ ํ, ๋ชจ๋  ํต์ ์ด ๋๋ฌ๋ค๋ฉด ํด์ ํด์ผ ํ๋ค.

[![img](https://camo.githubusercontent.com/8bb8960e46a3bfada6a237a7a91bce75a0a3e0e34eab5c1f5143ca6fe34d0b5f/68747470733a2f2f6d656469612e6765656b73666f726765656b732e6f72672f77702d636f6e74656e742f75706c6f6164732f434e2e706e67)](https://camo.githubusercontent.com/8bb8960e46a3bfada6a237a7a91bce75a0a3e0e34eab5c1f5143ca6fe34d0b5f/68747470733a2f2f6d656469612e6765656b73666f726765656b732e6f72672f77702d636f6e74656e742f75706c6f6164732f434e2e706e67)

1. ํด๋ผ์ด์ธํธ๋ ์๋ฒ์๊ฒ ์ฐ๊ฒฐ์ ์ข๋ฃํ๋ค๋ FIN ํ๋๊ทธ๋ฅผ ๋ณด๋ธ๋ค.
2. ์๋ฒ๋ FIN์ ๋ฐ๊ณ , ํ์ธํ๋ค๋ ACK๋ฅผ ํด๋ผ์ด์ธํธ์๊ฒ ๋ณด๋ธ๋ค. (์ด๋ ๋ชจ๋  ๋ฐ์ดํฐ๋ฅผ ๋ณด๋ด๊ธฐ ์ํด CLOSE_WAIT ์ํ๊ฐ ๋๋ค)
3. ๋ฐ์ดํฐ๋ฅผ ๋ชจ๋ ๋ณด๋๋ค๋ฉด, ์ฐ๊ฒฐ์ด ์ข๋ฃ๋์๋ค๋ FIN ํ๋๊ทธ๋ฅผ ํด๋ผ์ด์ธํธ์๊ฒ ๋ณด๋ธ๋ค.
4. ํด๋ผ์ด์ธํธ๋ FIN์ ๋ฐ๊ณ , ํ์ธํ๋ค๋ ACK๋ฅผ ์๋ฒ์๊ฒ ๋ณด๋ธ๋ค. (์์ง ์๋ฒ๋ก๋ถํฐ ๋ฐ์ง ๋ชปํ ๋ฐ์ดํฐ๊ฐ ์์ ์ ์์ผ๋ฏ๋ก TIME_WAIT์ ํตํด ๊ธฐ๋ค๋ฆฐ๋ค.)

- ์๋ฒ๋ ACK๋ฅผ ๋ฐ์ ์ดํ ์์ผ์ ๋ซ๋๋ค (Closed)
- TIME_WAIT ์๊ฐ์ด ๋๋๋ฉด ํด๋ผ์ด์ธํธ๋ ๋ซ๋๋ค (Closed)

์ด๋ ๊ฒ 4๋ฒ์ ํต์ ์ด ์๋ฃ๋๋ฉด ์ฐ๊ฒฐ์ด ํด์ ๋๋ค.



#### ๐ก 3-way handshaking ๊ณผ์ ์์ ํด๋ผ์ด์ธํธ๊ฐ ์๋ฒ๊ฐ ๋ณด๋ธ ACK+SYN์ ๋ฐ์ง ๋ชปํ๋ฉด? - ์๋ฒ ์ฌํ

- ํด๋ผ์ด์ธํธ์์ ํน์  ์๊ฐ์ ๋๊ธฐํด๋ ์ ์ก์ด ์๋๋ ๊ฒฝ์ฐ, ์์ฒญ SYN์ ์ฌ์ ์ก 

  

#### ๐ก UDP์์ ์ ๋ขฐ๋๋ฅผ ๋ณด์ฅํ๋ ๋ฐฉ๋ฒ์ ์ค๋ชํด์ฃผ์ธ์.

- ๋ฐ์ /์์  IP ๋ฐ ํ๋กํ ์ฝ์์ ์ฒดํฌ์ฌ์ ๊ณ์ฐํ๋ค.



## [HTTP์ HTTPS](#http์-https-๋ต๋ณ)
#### ๐ก HTTP์ HTTPS๋ฅผ ์ค๋ชํด์ฃผ์ธ์

- ##### HTTP ํ๋กํ ์ฝ

  - ๊ฐ๋

    - HyperText Transfer Protocol
    - ์น ์์์ ํด๋ผ์ด์ธํธ์ ์๋ฒ ๊ฐ์ ์์ฒญ/์๋ต(request/response)์ผ๋ก ์ ๋ณด๋ฅผ ์ฃผ๊ณ  ๋ฐ์ ์ ์๋ ํ๋กํ ์ฝ

  - ํน์ง

    - ์ฃผ๋ก HTML ๋ฌธ์๋ฅผ ์ฃผ๊ณ ๋ฐ๋ ๋ฐ์ ์ฐ์ธ๋ค.

    - TCP์ UDP๋ฅผ ์ฌ์ฉํ๋ฉฐ, **80๋ฒ ํฌํธ**๋ฅผ ์ฌ์ฉํ๋ค.

    - 1. ๋น์ฐ๊ฒฐ(Connectionless)

      - ํด๋ผ์ด์ธํธ๊ฐ ์์ฒญ์ ์๋ฒ์ ๋ณด๋ด๊ณ  ์๋ฒ๊ฐ ์ ์ ํ ์๋ต์ ํด๋ผ์ด์ธํธ์ ๋ณด๋ด๋ฉด ๋ฐ๋ก ์ฐ๊ฒฐ์ด ๋๊ธด๋ค.

    - 1. ๋ฌด์ํ(Stateless)

      - ์ฐ๊ฒฐ์ ๋๋ ์๊ฐ ํด๋ผ์ด์ธํธ์ ์๋ฒ์ ํต์ ์ ๋๋๋ฉฐ ์ํ ์ ๋ณด๋ฅผ ์ ์งํ์ง ์๋๋ค.

- **HTTPS ํ๋กํ ์ฝ**

  - ๊ฐ๋
    - HyperText Transfer Protocol over Secure Socket Layer
      - ๋๋ HTTP over TLS, HTTP over SSL, HTTP Secure
    - ์น ํต์  ํ๋กํ ์ฝ์ธ HTTP์ ๋ณด์์ด ๊ฐํ๋ ๋ฒ์ ์ ํ๋กํ ์ฝ
  - ํน์ง
    - HTTPS์ ๊ธฐ๋ณธ TCP/IP ํฌํธ๋ก **443๋ฒ ํฌํธ**๋ฅผ ์ฌ์ฉํ๋ค.
    - HTTPS๋ ์์ผ ํต์ ์์ ์ผ๋ฐ ํ์คํธ๋ฅผ ์ด์ฉํ๋ ๋์ ์, ์น ์์์ ์ ๋ณด๋ฅผ ์ํธํํ๋ SSL์ด๋ TLS ํ๋กํ ์ฝ์ ํตํด ์ธ์ ๋ฐ์ดํฐ๋ฅผ ์ํธํํ๋ค.
      - TLS(Transport Layer Security) ํ๋กํ ์ฝ์ SSL(Secure Socket Layer) ํ๋กํ ์ฝ์์ ๋ฐ์ ํ ๊ฒ์ด๋ค.
      - ๋ ํ๋กํ ์ฝ์ ์ฃผ์ ๋ชฉํ๋ ๊ธฐ๋ฐ์ฑ(์ฌ์ํ ๋ณดํธ), ๋ฐ์ดํฐ ๋ฌด๊ฒฐ์ฑ, ID ๋ฐ ๋์งํธ ์ธ์ฆ์๋ฅผ ์ฌ์ฉํ ์ธ์ฆ์ ์ ๊ณตํ๋ ๊ฒ์ด๋ค.
    - ๋ฐ๋ผ์ ๋ฐ์ดํฐ์ ์ ์ ํ ๋ณดํธ๋ฅผ ๋ณด์ฅํ๋ค.
      - ๋ณดํธ์ ์์ค์ ์น ๋ธ๋ผ์ฐ์ ์์์ ๊ตฌํ ์ ํ๋์ ์๋ฒ ์ํํธ์จ์ด, ์ง์ํ๋ ์ํธํ ์๊ณ ๋ฆฌ์ฆ์ ๋ฌ๋ ค์๋ค.
    - ๊ธ์ต ์ ๋ณด๋ ๋ฉ์ผ ๋ฑ ์ค์ํ ์ ๋ณด๋ฅผ ์ฃผ๊ณ ๋ฐ๋ ๊ฒ์ HTTPS๋ฅผ, ์๋ฌด๋ ๋ด๋ ์๊ด ์๋ ํ์ด์ง๋ HTTP๋ฅผ ์ฌ์ฉํ๋ค.



#### ๐ก HTTP์ ๋จ์ ์ ์ค๋ชํด์ฃผ์ธ์

- ์น ํ์ด์ง(HTML)๋ ํ์คํธ์ด๊ณ , HTTP๋ฅผ ํตํด ์ด๋ฐ ํ์คํธ ์ ๋ณด๋ฅผ ๊ตํํ๋ ๊ฒ์ด๋ค.

- ์ด๋ ์ฃผ๊ณ ๋ฐ๋ ํ์คํธ ์ ๋ณด์ ์ฃผ๋ฏผ๋ฑ๋ก๋ฒํธ๋ ๋น๋ฐ๋ฒํธ์ ๊ฐ์ด ๋ฏผ๊ฐํ ์ ๋ณด๊ฐ ํฌํจ๋ ์ํ์์ ๋คํธ์ํฌ ์์์ ์ค๊ฐ์ ์ 3์๊ฐ ์ ๋ณด๋ฅผ ๊ฐ๋ก์ฑ๋ค๋ฉด ๋ณด์์ ํฐ ๋ฌธ์ ๊ฐ ๋ฐ์ํ๋ค.

- ์ฆ, ์ค๊ฐ์์ ์ ๋ณด๋ฅผ ๋ณผ ์ ์๋๋ก ์ฃผ๊ณ ๋ฐ๋ ์ ๋ณด๋ฅผ ์ํธํํ๋ ๋ฐฉ๋ฒ์ธ HTTPS๋ฅผ ์ฌ์ฉํ๋ ๊ฒ์ด๋ค.

  

#### ๐ก HTTP 1.0+์ HTTP1.1์ HTTP2.0 ์ฐจ์ด์ ์ ๋ฌด์์ธ๊ฐ์?





#### ๐ก HTTP๋ ์ ๋น์ฐ๊ฒฐ์ฑ์ธ๊ฐ? - ์๋ฒ ์ฌํ

- ์น ํ์ด์ง๋ฅผ ๋ณด๋ ์ค ์ธํฐ๋ท ์ฐ๊ฒฐ์ด ๋๊ฒผ๋ค๊ฐ ๋ค์ ์ฐ๊ฒฐ๋์ด๋ ํ์ด์ง๋ฅผ ๊ณ์ ๋ณผ ์ ์๊ฒ ํ๊ธฐ ์ํด์

  

#### ๐ก ๋ชจ๋  ์น ํ์ด์ง์์ HTTPS ๋ฅผ ์ฌ์ฉํ์ง ์๋ ์ด์ ๋ฅผ ์ค๋ชํด์ฃผ์ธ์.

- ์ํธํ๋ฅผ ํ๋ ๊ณผ์ ์ด ์น ์๋ฒ์ ๋ถํ๋ฅผ ์ค๋ค.

- HTTPS๋ ์ค์น ๋ฐ ์ธ์ฆ์๋ฅผ ์ ์งํ๋๋ฐ ์ถ๊ฐ ๋น์ฉ์ด ๋ฐ์ํ๋ค.

- HTTP์ ๋นํด ๋๋ฆฌ๋ค.

- ์ธํฐ๋ท ์ฐ๊ฒฐ์ด ๋๊ธด ๊ฒฝ์ฐ ์ฌ์ธ์ฆ ์๊ฐ์ด ์์๋๋ค

  

#### ๐ก ๋น๋์นญํค ๋๋ ๊ณต๊ฐํค ์ํธํ ๋ฐฉ์์ ๋ฌด์์ธ๊ฐ์?

- A๋ ๊ณต๊ฐํค์ ๊ฐ์ธํค๋ฅผ ์์ฑํ๋ค.
- B๋ A์ ๊ณต๊ฐํค๋ฅผ ์กฐํํ๊ณ  A์ ๊ณต๊ฐํค๋ฅผ ์ด์ฉํด์ ๋ฐ์ดํฐ๋ฅผ ์ํธํํ ํ ์ ์กํ๋ค.
- A๋ ๊ฐ์ธํค๋ก ์ํธํ๋ ๋ฐ์ดํฐ๋ฅผ ๋ณตํธํํ๋ค.



#### ๐ก HTTP REQUEST ๋ฐฉ์ ์ค GET๊ณผ POST์ ์ฐจ์ด์ ์ค๋ชํด์ฃผ์ธ์.

> HTTP ํ๋กํ ์ฝ์ ์ด์ฉํด์ ์๋ฒ์ ๋ฐ์ดํฐ(์์ฒญ ์ ๋ณด)๋ฅผ ์ ๋ฌํ  ๋ ์ฌ์ฉํ๋ ๋ฐฉ์
>
> **์ฌ์ฉ๋ชฉ์ , ์์ฒญ์ body ์ ๋ฌด, ๋ฉฑ๋ฑ์ฑ(GET์ ๋ฉฑ๋ฑ)**

- GET ๋ฉ์๋ ๋ฐฉ์

  - ๊ฐ๋

    - ์ ๋ณด๋ฅผ ์กฐํํ๊ธฐ ์ํ ๋ฉ์๋
    - ์๋ฒ์์ ์ด๋ค ๋ฐ์ดํฐ๋ฅผ ๊ฐ์ ธ์์ ๋ณด์ฌ์ฃผ๊ธฐ ์ํ ์ฉ๋์ ๋ฉ์๋
    - **๊ฐ์ ธ์ค๋ ๊ฒ(Select)**

  - ์ฌ์ฉ ๋ฐฉ๋ฒ

    - URL์ ๋์ '?'๊ฐ ๋ถ๊ณ , ์์ฒญ ์ ๋ณด๊ฐ (key=value)ํํ์ ์์ ์ด๋ฃจ์ด ?๋ค์ ์ด์ด์ ๋ถ์ด ์๋ฒ๋ก ์ ์กํ๋ค.

    - ์์ฒญ ์ ๋ณด๊ฐ ์ฌ๋ฌ ๊ฐ์ผ ๊ฒฝ์ฐ์๋ '&'๋ก ๊ตฌ๋ถํ๋ค.

      Ex) `www.urladdress.xyz?name1=value1&name2=value2`

  - ํน์ง

    - URL์ ์์ฒญ ์ ๋ณด๋ฅผ ๋ถ์ฌ์ ์ ์กํ๋ค.

    - URL์ ์์ฒญ ์ ๋ณด๊ฐ ์ด์ด๋ถ๊ธฐ ๋๋ฌธ์ ๊ธธ์ด ์ ํ์ด ์์ด์ ๋์ฉ๋์ ๋ฐ์ดํฐ๋ฅผ ์ ์กํ๊ธฐ ์ด๋ ต๋ค.

      - ํ ๋ฒ ์์ฒญ ์ ์ ์ก ๋ฐ์ดํฐ(์ฃผ์๊ฐ + ํ๋ผ๋ฏธํฐ)์ ์์ 255์๋ก ์ ํ๋๋ค.(HTTP/1.1์ 2048์)

    - ์์ฒญ ์ ๋ณด๋ฅผ ์ฌ์ฉ์๊ฐ ์ฝ๊ฒ ๋์ผ๋ก ํ์ธํ  ์ ์๋ค.

      - POST ๋ฐฉ์๋ณด๋ค ๋ณด์์ ์ทจ์ฝํ๋ค.

    - HTTP ํจํท์ Body๋ ๋น์ด ์๋ ์ํ๋ก ์ ์กํ๋ค.

      

- POST ๋ฉ์๋ ๋ฐฉ์

  - ๊ฐ๋

    - ์๋ฒ์ ๊ฐ์ด๋ ์ํ๋ฅผ ๋ฐ๊พธ๊ธฐ ์ํ ์ฉ๋์ ๋ฉ์๋
    - **์ํํ๋ ๊ฒ(Insert, Update, Delete)**

  - ์ฌ์ฉ ๋ฐฉ๋ฒ

    - ์์ฒญ ์ ๋ณด๋ฅผ HTTP ํจํท์ Body ์์ ์จ๊ฒจ์ ์๋ฒ๋ก ์ ์กํ๋ค.

    - Request Header์ Content-Type์ ํด๋น ๋ฐ์ดํฐ ํ์์ด ํํ๋๋ฉฐ, ์ ์กํ๊ณ ์ ํ๋ ๋ฐ์ดํฐ ํ์์ ์ ์ด์ฃผ์ด์ผ ํ๋ค.

  - ํน์ง

    - Body ์์ ์จ๊ฒจ์ ์์ฒญ ์ ๋ณด๋ฅผ ์ ์กํ๊ธฐ ๋๋ฌธ์ ๋์ฉ๋์ ๋ฐ์ดํฐ๋ฅผ ์ ์กํ๊ธฐ์ ์ ํฉํ๋ค.

    - ํด๋ผ์ด์ธํธ ์ชฝ์์ ๋ฐ์ดํฐ๋ฅผ ์ธ์ฝ๋ฉํ์ฌ ์๋ฒ๋ก ์ ์กํ๊ณ , ์ด๋ฅผ ๋ฐ์ ์๋ฒ ์ชฝ์ด ํด๋น ๋ฐ์ดํฐ๋ฅผ ๋์ฝ๋ฉํ๋ค.

    - GET ๋ฐฉ์๋ณด๋ค ๋ณด์์ ์์ ํ๋ค.

      

#### ๐ก GET, POST๋ฅผ ์ ์ธํ๊ณ  ๋ค๋ฅธ ๋ฐฉ์๋ค์ ์ค๋ชํด์ฃผ์ธ์.

```
OPTION : ํต์ ๊ณผ ๊ด๋ จ๋ ์ ํ์ฌํญ๋ค์ ๋ํ ์ ๋ณด๋ฅผ ์๊ตฌํ๋ ๊ฒฝ์ฐ
PUT : Request ๋ฉ์์ง์ ํฌํจ๋์ด ์๋ data๋ฅผ ์ง์ ํ Request-URI๋ก ์ ์ฅํ๊ธฐ ์ํจ
DELETE : ํน์  resource๋ฅผ ์ง์ฐ๊ธฐ ์ํจ
TRACE : ์ต์ข destination๊น์ง์ Loopback์ ํ์คํธํ๊ธฐ ์ํจ (์๋ฒ๊ฐ ์ด๋ค ํ๋ก์๋ฅผ ๊ฑฐ์ณ์๋์ง ๊ณผ์ ์ ๋ฐํ)
```



#### ๐ก ์กฐํํ๊ธฐ ์ํ ์ฉ๋ POST๊ฐ ์๋ GET ๋ฐฉ์์ ์ฌ์ฉํ๋ ์ด์ ?  

> **๋ฉฑ๋ฑ์ฑ** ๋๋ฌธ์ด๋ค
>
> GET์ ๋ฌธ์ ๊ฐ ์๊ฒจ๋ ์ฌ๋ฌ๋ฒ ๋ณด๋ผ ์ ์๋ค. ๋๋จธ์ง ๋ฐฉ์์ ์๋๋ค.

1. ์ค๊ณ ์์น์ ๋ฐ๋ผ GET ๋ฐฉ์์ ์๋ฒ์๊ฒ ์ฌ๋ฌ ๋ฒ ์์ฒญ์ ํ๋๋ผ๋ ๋์ผํ ์๋ต์ด ๋์์์ผ ํ๋ค.

   - GET ๋ฐฉ์์ **๊ฐ์ ธ์ค๋ ๊ฒ(Select)** ์ผ๋ก, ์๋ฒ์ ๋ฐ์ดํฐ๋ ์ํ๋ฅผ ๋ณ๊ฒฝ์ํค์ง ์์์ผ ํ๋ค.

2. ์น์์ ๋ชจ๋  ๋ฆฌ์์ค๋ Linkํ  ์ ์๋ URL์ ๊ฐ์ง๊ณ  ์์ด์ผ ํ๋ค.

   - ์ด๋ค ์นํ์ด์ง๋ฅผ ๋ณด๊ณ  ์์ ๋ ๋ค๋ฅธ ์ฌ๋ํํ ๊ทธ ์ฃผ์๋ฅผ ์ฃผ๊ธฐ ์ํด์ ์ฃผ์์ฐฝ์ URL์ ๋ณต์ฌํด์ ์ค ์ ์์ด์ผ ํ๋ค.

   - ์ด๋ POST ๋ฐฉ์์ ์ฌ์ฉํ  ๊ฒฝ์ฐ์ ๊ฐ(๋งํฌ์ ์ ๋ณด)์ด Body์ ์๊ธฐ ๋๋ฌธ์ URL๋ง ์ ๋ฌํ  ์ ์์ผ๋ฏ๋ก GET ๋ฐฉ์์ ์ฌ์ฉํด์ผํ๋ค. ๊ทธ๋ฌ๋ ๊ธ์ ์ ์ฅํ๋ ๊ฒฝ์ฐ์๋ URL์ ์ ๊ณตํ  ํ์๊ฐ ์๊ธฐ ๋๋ฌธ์ POST ๋ฐฉ์์ ์ฌ์ฉํ๋ค.

     

#### ๐ก ํ๋ ์น ์์๋ ๋น์ฐ๊ฒฐ์ฑ์ ํด๊ฒฐ๋ฐฉ๋ฒ์ ์ค๋ชํด์ฃผ์ธ์. - ์๋ฒ ์ฌํ

- *์ฟ ํค, ์ธ์, ํ ํฐ*์ ์ฌ์ฉ



## [๋ก๋๋ฐธ๋ฐ์](#๋ก๋๋ฐธ๋ฐ์-๋ต๋ณ) - ์๋ฒ ๊ฐ๋ฐ์๋ง ๋ต๋ณํ  ๊ฒ
#### ๐ก ๋ก๋ ๋ฐธ๋ฐ์ฑ์ ์ค๋ชํด์ฃผ์ธ์.  

> ๋ ์ด์์ CPU or ์ ์ฅ์ฅ์น์ ๊ฐ์ ์ปดํจํฐ ์์๋ค์๊ฒ ์์์ ๋๋๋ ๊ฒ

- **๋ก๋ ๋ฐธ๋ฐ์ฑ**์ ๋ถ์ฐ์ ์น ์๋น์ค๋ก, ์ฌ๋ฌ ์๋ฒ์ ๋ถํ(Load)๋ฅผ ๋๋์ด์ฃผ๋ ์ญํ ์ ํ๋ค. 
- Load Balancer๋ฅผ ํด๋ผ์ด์ธํธ์ ์๋ฒ ์ฌ์ด์ ๋๊ณ , ๋ถํ๊ฐ ์ผ์ด๋์ง ์๋๋ก ์ฌ๋ฌ ์๋ฒ์ ๋ถ์ฐ์์ผ์ฃผ๋ ๋ฐฉ์์ด๋ค. 
- ์๋น์ค๋ฅผ ์ด์ํ๋ ์ฌ์ดํธ์ ๊ท๋ชจ์ ๋ฐ๋ผ ์น ์๋ฒ๋ฅผ ์ถ๊ฐ๋ก ์ฆ์คํ๋ฉด์ ๋ก๋ ๋ฐธ๋ฐ์๋ก ๊ด๋ฆฌํด์ฃผ๋ฉด ์น ์๋ฒ์ ๋ถํ๋ฅผ ํด๊ฒฐํ  ์ ์๋ค.

#### ๐ก L4 ๋ก๋ ๋ฐธ๋ฐ์ฑ๊ณผ L7 ๋ก๋ ๋ฐธ๋ฐ์ฑ์ ๋ํด ์ค๋ชํ๊ณ , ์ฐจ์ด๋ฅผ ๋งํด๋ณด์ธ์  

- L4 ๋ก๋ ๋ฐธ๋ฐ์ฑ
  - ์ฃผ๋ก **Round Robin** ๋ฐฉ์์ ์ฌ์ฉํ๋ฉฐ, **๋คํธ์ํฌ ๊ณ์ธต(IP, IPX)์ด๋ ํธ๋์คํฌํธ ๊ณ์ธต(TCP, UDP)์ ์ ๋ณด**๋ฅผ ๋ฐํ์ผ๋ก ๋ก๋๋ฅผ ๋ถ์ฐ์ํจ๋ค.
- L7 ๋ก๋ ๋ฐธ๋ฐ์ฑ
  - **์ ํ๋ฆฌ์ผ์ด์ ๊ณ์ธต(HTTP, FTP, SMTP)์์ ๋ก๋๋ฅผ ๋ถ์ฐ**ํ๊ธฐ ๋๋ฌธ์ HTTP ํค๋, ์ฟ ํค ๋ฑ๊ณผ ๊ฐ์ ์ฌ์ฉ์์ ์์ฒญ์ ๊ธฐ์ค์ผ๋ก ํน์  ์๋ฒ์ ํธ๋ํฝ์ ๋ถ์ฐํ๋ ๊ฒ์ด ๊ฐ๋ฅํ๋ค.
  - **ํจํท์ ๋ด์ฉ์ ํ์ธํ๊ณ  ๊ทธ ๋ด์ฉ์ ๋ฐ๋ผ ๋ก๋๋ฅผ ํน์  ์๋ฒ์ ๋ถ๋ฐฐํ๋ ๊ฒ์ด ๊ฐ๋ฅํ ๊ฒ**

|               | L4 ๋ก๋๋ฐธ๋ฐ์                                                | L7 ๋ก๋๋ฐธ๋ฐ์                                                |
| ------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ๋คํธ์ํฌ ๊ณ์ธต | ์ ์ก๊ณ์ธต                                                     | ์์ฉ๊ณ์ธต                                                     |
| ํน์ง          | TCP/UDP ํฌํธ ์ ๋ณด๋ฅผ ๋ฐํ์ผ๋ก                                 | TCP/UDP ํฌํธ ์ ๋ณด + HTTP์ URI, FTP์ ํ์ผ๋ช, ์ฟ ํค ์ ๋ณด ๋ฑ์ ๋ฐํ์ผ๋ก |
| ์ฅ์           | 1. ์๋๊ฐ ๋น ๋ฅด๊ณ  ํจ์จ์ด ๋์<br /> 2. ๋ฐ์ดํฐ์ ๋ด์ฉ์ ๋ณตํธํํ  ํ์๊ฐ ์์ด์ ์์ ํจ<br />3. L7 ๋ก๋ ๋ฐธ๋ฐ์๋ณด๋ค ๊ฐ๊ฒฉ์ด ์ ๋ ดํจ | 1. ์์ ๊ณ์ธต์์ ๋ก๋๋ฅผ ๋ถ์ฐํ๊ธฐ ๋๋ฌธ์ ๋ ์ฌ์ธํ ๋ผ์ฐํ์ด ๊ฐ๋ฅํจ<br />2. ์บ์ฑ ๊ธฐ๋ฅ์ ์ ๊ณตํจ<br />3. ๋น์ ์์ ์ธ ํธ๋ํฝ์ ์ฌ์ ์ ํํฐ๋งํ  ์ ์์ด ์๋น์ค ์์ ์ฑ์ด ๋์ |
| ๋จ์           | 1. ํจํท์ ๋ด์ฉ์ ๋ณผ ์ ์๊ธฐ ๋๋ฌธ์ ์ฌ์ธํ ๋ผ์ฐํ์ด ๋ถ๊ฐ๋ฅ<br />2. ์ฌ์ฉ์์ IP๊ฐ ์์๋ก ๋ฐ๋๋ ๊ฒฝ์ฐ, ์ฐ์์ ์ธ ์๋น์ค ์ ๊ณต์ด ์ด๋ ค์ | 1. ํจํท์ ๋ด์ฉ์ ๋ณตํธํํด์ผ ํ๊ธฐ์ ๋ ๋์ ๋น์ฉ์ ์ง๋ถํด์ผํจ<br />2. ํด๋ผ์ด์ธํธ๊ฐ ๋ก๋๋ฐธ๋ฐ์์ ์ธ์ฆ์๋ฅผ ๊ณต์ ํ๊ธฐ ๋๋ฌธ์ ๊ณต๊ฒฉ์๊ฐ ๋ก๋๋ฐธ๋ฐ์๋ฅผ ํตํด ๋ฐ์ดํฐ์ ์ ๊ทผํ  ๋ณด์ ์์ ์ํ์ฑ ์กด์ฌ |



#### ๐ก ๊ฒ์ดํธ์จ์ด๋?  

- ํ ๋คํธ์ํฌ(segment)์์ ๋ค๋ฅธ ๋คํธ์ํฌ๋ก ์ด๋ํ๊ธฐ ์ํ์ฌ ๊ฑฐ์ณ์ผ ํ๋ ์ง์ ์๋๋ค.

  

#### ๐ก ์๋ฒ์ ํธ๋ํฝ์ด ์ฃผ์ด์ก์ ๋ ์ด๋ป๊ฒ ์๋ต์๋๋ฅผ ๊ฐ์ ํ  ์ ์๋๊ฐ?  



#### ๐ก ํ๋ผ์ด๋น ์๋ธ๋ท๊ณผ ํผ๋ธ๋ฆญ ์๋ธ๋ท์ ์ฐจ์ด

- **ํผ๋ธ๋ฆญ ์๋ธ๋ท**์ ์ธ๋ถ์์ ์ง์  IP๋ฅผ ์ฐ์ด์ ๋ค์ด์ฌ ์ ์๋ **์๋ธ๋ท**์ด๊ณ , **ํ๋ผ์ด๋น ์๋ธ๋ท**์ ๋ค๋ฅธ ์์(Load balancer,Proxy ๋ฑ)์ ํตํ์ง ์์ผ๋ฉด ๋ค์ด์ฌ ์ ์๋ค.

