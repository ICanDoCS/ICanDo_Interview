

## [OSI 7 layers์ TCP/IP 4 layer](#osi-7-layers์-tcpip-4-layers-๋ต๋ณ)
#### ๐ก OSI 7 Layer ๋๋ TCP/IP Layer์ ๊ฐ ๊ณ์ธต์ ๋ํ ์ค๋ช์ ํด์ฃผ์ธ์.

ํ๋์ ์น ๋ชจ๋ธ์ TCP/IP๋ก ๋์ด์ค๊ฒ ๋์์
```
Application Layer : TCP/IP ์์ผ ํ๋ก๊ทธ๋๋ฐ์์ ์ ๊ณตํ๋ API๋ฅผ ํ์ฌ ํต์ ๊ฐ๋ฅํ ํ๋ก๊ทธ๋จ์ ํ์ฉํ  ์ ์๋ ๊ณ์ธต

ํ๋กํ ์ฝ โ FTP, HTTP, SSH

Transport Layer : ํต์  ๋ธ๋ ๊ฐ์ ์ฐ๊ฒฐ์ ์ ์ดํ๊ณ , ์ ๋ขฐ์ฑ ์๋ ๋ฐ์ดํฐ ์ ์ก์ ๋ด๋นํ๋ค.

ํ๋กํ ์ฝ โ TCP, UDP

Internet Layer : ํต์  ๋ธ๋ ๊ฐ์ IPํจํท์ ์ ์กํ๋ ๊ธฐ๋ฅ๊ณผ ๋ผ์ฐํ ๊ธฐ๋ฅ์ ๋ด๋นํ๋ค.

ํ๋กํ ์ฝ โ IP, ARP, RARP

Network Access Layer : 

OSI 7๊ณ์ธต์ ๋ฌผ๋ฆฌ๊ณ์ธต๊ณผ ๋ฐ์ดํฐ ๋งํฌ ๊ณ์ธต์ ํด๋นํ๋ค.

๋ฌผ๋ฆฌ์ ์ธ ์ฃผ์๋ก MAC์ ์ฌ์ฉํ๋ค.

```

#### ๐ก OSI 7 Layer ๋๋ TCP/IP Layer์์ ๊ณ์ธตํํ๋ ์ด์ ๊ฐ ๋ฌด์์ธ๊ฐ์?

```
1.๊ณ์ธต์ ๋ถ๋ฆฌํจ์ผ๋ก์ ๊ฐ ๊ณ์ธต์ ๋๋ฆฝ์ ์ธ ์ญํ  ์ํ
2.์ญํ ์ด ๋ถ๋ฆฌ๋๋ฉด์ ๋ฌธ์  ๋ฐ์์ ๋ฌธ์ ์ ํ์์ ๋ณด์์ ๋ ์ด๋ค ๊ณ์ธต์ธ์ง ํ์ ๊ฐ๋ฅ
```

<del>#### ๐ก Encapsulation๊ณผ Decapsulation์ ์๋ก ๋น๊ตํ๋ฉฐ ์ค๋ชํด์ฃผ์ธ์ </del>

#### ๐ก IP ์ฃผ์ ๋ฐ MAC ์ฃผ์๋?
```
IP ์ฃผ์๋ ๋คํธ์ํฌ ํต์ ์ ์์ด์ ๊ฐ๊ฐ์ ํต์ ๊ธฐ๊ธฐ(์ปดํจํฐ, ๋ธํธ๋ถ, ์ค๋งํธํฐ ๋ฑ)์ ํ ๋น๋ ์๋ณ๋ฒํธ
MAC ์ฃผ์๋ ํต์ ๊ธฐ๊ธฐ์ ํ๋์จ์ด ์์ฒด์ ๋ถ์ฌ๋ ๊ณ ์ ํ ์๋ณ๋ฒํธ
```

#### ๐ก IPV4 vs IPV6 ์ ์ค๋ชํด์ฃผ์ธ์.

```
- ์ง์ฐ์ ๋ฏผ๊ฐํ ํจํท์ ๊ตฌ๋ถํ๋ ๊ธฐ๋ณธ์ ์ธ QoS(Quality of Service)
- NAT๋ฅผ ์์ฐ์ผ๋ก์จ ์ฃผ์ ๊ณต๊ฐ์ 32๋นํธ์์ 128๋นํธ๋ก ํ์ฅ
- ๋คํธ์ํฌ ๋ ์ด์ด ๋ณด์ ๋ด์ฅ(IPsec)
- ์์ฌ์ด ๋คํธ์ํฌ ๊ด๋ฆฌ๋ฅผ ์ํ ๋ฌด์ํ ์ฃผ์ ์๋ ๊ตฌ์ฑ
- ์ฒ๋ฆฌ ์ค๋ฒํค๋๊ฐ ์ค์ด๋  ๊ฐ์ ๋ ํค๋ ๊ตฌ์กฐ
```

#### ๐ก IPv4์ ์ฃผ์ ๋ถ์กฑํ์์ ํด๊ฒฐํ๊ธฐ ์ํด ํ์ฌ ์ด๋ค ๋ฐฉ๋ฒ์ ์ฌ์ฉํ๊ณ  ์๋์? - ์ฌํ

## [TCP์ UDP](#tcp์-udp-๋ต๋ณ)
#### ๐ก TCP์ UDP์ ํน์ง๊ณผ ์ฐจ์ด์ ์ ์ค๋ชํด์ฃผ์ธ์.

```
TCP
- ์ฐ๊ฒฐํ ์๋น์ค๋ก ๊ฐ์ ํ์  ๋ฐฉ์์ ์ ๊ณตํ๋ค.
- 3-way handshaking๊ณผ์ ์ ํตํด ์ฐ๊ฒฐ์ ์ค์ ํ๊ณ  4-way handshaking์ ํตํด ํด์ ํ๋ค.
- ํ๋ฆ ์ ์ด ๋ฐ ํผ์ก ์ ์ด.
- ๋์ ์ ๋ขฐ์ฑ์ ๋ณด์ฅํ๋ค.
- UDP๋ณด๋ค ์๋๊ฐ ๋๋ฆฌ๋ค.

ํน์ง
- ์๋ฒ์์ผ์ ์ฐ๊ฒฐ๋ง์ ๋ด๋นํ๋ค.
- ์ฐ๊ฒฐ๊ณผ์ ์์ ๋ฐํ๋ ํด๋ผ์ด์ธํธ ์์ผ์ ๋ฐ์ดํฐ์ ์ก์์ ์ ์ฌ์ฉ๋๋คํ ์๋น์ค๋ก ๊ฐ์ ํ์  ๋ฐฉ์์ ์ ๊ณตํ๋ค.
- ์๋ฒ์ ํด๋ผ์ด์ธํธ๋ 1๋1๋ก ์ฐ๊ฒฐ๋๋ค.
- ์คํธ๋ฆผ ์ ์ก์ผ๋ก ์ ์ก ๋ฐ์ดํฐ์ ํฌ๊ธฐ๊ฐ ๋ฌด์ ํ์ด๋ค.
- ํจํท์ ๋ํ ์๋ต์ ํด์ผํ๊ธฐ ๋๋ฌธ์(์๊ฐ ์ง์ฐ, CPU ์๋ชจ) ์ฑ๋ฅ์ด ๋ฎ๋ค.
- Streaming ์๋น์ค์ ๋ถ๋ฆฌํ๋ค.(์์ค๋ ๊ฒฝ์ฐ ์ฌ์ ์ก ์์ฒญ์ ํ๋ฏ๋ก)

UDP
- ๋น์ฐ๊ฒฐํ ์๋น์ค๋ก ๋ฐ์ดํฐ๊ทธ๋จ ๋ฐฉ์์ ์ ๊ณตํ๋ค
- ์ ๋ณด๋ฅผ ์ฃผ๊ณ  ๋ฐ์ ๋ ์ ๋ณด๋ฅผ ๋ณด๋ด๊ฑฐ๋ ๋ฐ๋๋ค๋ ์ ํธ์ ์ฐจ๋ฅผ ๊ฑฐ์น์ง ์๋๋ค.
- UDPํค๋์ CheckSum ํ๋๋ฅผ ํตํด ์ต์ํ์ ์ค๋ฅ๋ง ๊ฒ์ถํ๋ค.
- ์ ๋ขฐ์ฑ์ด ๋ฎ๋ค
- TCP๋ณด๋ค ์๋๊ฐ ๋น ๋ฅด๋ค

ํน์ง
- UDP์๋ ์ฐ๊ฒฐ ์์ฒด๊ฐ ์์ด์(connect ํจ์ ๋ถํ์) ์๋ฒ ์์ผ๊ณผ ํด๋ผ์ด์ธํธ ์์ผ์ ๊ตฌ๋ถ์ด ์๋ค.
- ์์ผ ๋์  IP๋ฅผ ๊ธฐ๋ฐ์ผ๋ก ๋ฐ์ดํฐ๋ฅผ ์ ์กํ๋ค.
- ์๋ฒ์ ํด๋ผ์ด์ธํธ๋ 1๋1, 1๋N, N๋M ๋ฑ์ผ๋ก ์ฐ๊ฒฐ๋  ์ ์๋ค.
- ๋ฐ์ดํฐ๊ทธ๋จ(๋ฉ์ธ์ง) ๋จ์๋ก ์ ์ก๋๋ฉฐ ๊ทธ ํฌ๊ธฐ๋ 65535๋ฐ์ดํธ๋ก, ํฌ๊ธฐ๊ฐ ์ด๊ณผํ๋ฉด ์๋ผ์ ๋ณด๋ธ๋ค.
- ํ๋ฆ์ ์ด(flow control)๊ฐ ์์ด์ ํจํท์ด ์ ๋๋ก ์ ์ก๋์๋์ง, ์ค๋ฅ๊ฐ ์๋์ง ํ์ธํ  ์ ์๋ค.
- ํ์ผ ์ ์ก๊ณผ ๊ฐ์ ์ ๋ขฐ์ฑ์ด ํ์ํ ์๋น์ค๋ณด๋ค ์ฑ๋ฅ์ด ์ค์์ ๋๋ ๊ฒฝ์ฐ์ ์ฌ์ฉ๋๋ค.

```

![UDPTCP](./TCPUDP.png)

#### ๐ก TCP๋ฅผ ์ฌ์ฉํ๋ ๋ํ์ ์ธ ํ๋กํ ์ฝ์ ๋ฌด์์ธ๊ฐ์?

```
HTTP ํต์ 
```

#### ๐ก 3-Handshaking๊ณผ 4-Handshaking์ ๊ณผ์ ์ ์ค๋ชํด์ฃผ์ธ์. 

```
3-Handshaking
- CLIENT์์ ์น ์๋ฒ๋ก ์ฐ๊ฒฐ์ ์ต์ด์๋์ ๋จผ์  SYN ํจํท์ ๋ณด๋๋๋ค.
- SYN ํจํท์ ๋ณด๋ธ CLIENT๋ SYN-SENT ์ํ๊ฐ ๋ฉ๋๋ค.
- SERVER์์ CLOSED๋ PORT๊ฐ ๋ซํ์๋ ์ํ๋ฅผ ๋ปํ๊ณ , ํฌํธ๊ฐ ์๋น์ค ๊ฐ๋ฅํ ์ํ์ธ LISTEN์ํ๋ก ๋ง๋ค์ด์ฃผ์ด์ผ ํฉ๋๋ค.
- LISTEN์ํ์์ CLIENT๋ถํฐ SYNํจํท์ ๋ฐ์ผ๋ฉด ์ด์ ๋ํ ์๋ต์ผ๋ก SYN + ACK ํจํท์ CLIENT๋ก ๋ณด๋๋๋ค.
- SERVER๋ CLIENT IP์ ๋ํด ํฌํธ SYN-RECEIVED ์ํ๋ก ์ ํ๋ฉ๋๋ค.
- SERVER๋ก๋ถํฐ SYN+ACK ํจํท์ ๋ฐ์ผ๋ฉด, CLIENT๋ ESTABLISHED์ํ๋ก ๋ณํ๊ฒ ๋๋ฉด์ ์ฐ๊ฒฐ์ ํ์ธํฉ๋๋ค.
- CLIENT๋ SERVER๋ก SYN์ ๋ํ ์๋ต์ผ๋ก ACKํจํท์ ๋ณด๋๋๋ค.
- SERVER๋ ์ด ACK ํจํท์ ๋ฐ๊ณ  ํด๋น CLIENT IP์ ๋ํ ํฌํธ ESTABLISHED์ํ๋ก ์ ํ๋ฉ๋๋ค.
```
![3hands](./3hands.png)

```
4-Handshaking
1) ํด๋ผ์ด์ธํธ์์ ์๋ฒ์์ ์ฐ๊ฒฐ ์ข๋ฃ๋ฅผ ์ํด ์๋ฒ์ FIN ํจํท์ ๋ณด๋ด๊ณ  FIN_WAIT1 ์ํ๊ฐ ๋ฉ๋๋ค.
2) ์๋ฒ๋ ํด๋ผ์ด์ธํธ๋ก๋ถํฐ FIN์ ๋ฐ๊ณ  ์๋ต ํจํท ACK์ ๋ณด๋๋๋ค. 
์ํ๋ CLOSE_WAIT๊ฐ ๋ฉ๋๋ค
3) ์๋ฒ๊ฐ ํต์ ์ด ๋๋๋ฉด, ์ฆ ์ฐ๊ฒฐ์ ์ข๋ฃํ  ์ค๋น๊ฐ ๋๋ฉด ํด๋ผ์ด์ธํธ์๊ฒ FINํจํท์ ๋ณด๋ด๊ณ  LAST_WAIT ์ํ๊ฐ ๋ฉ๋๋ค  
4) ํด๋ผ์ด์ธํธ๋ ํ์ธ ํจํท ACK์ ๋ณด๋ด๊ณ  TIME_WAIT ์ํ๊ฐ ๋ฉ๋๋ค.

```
![4hands](./4hands.jpeg)


#### ๐ก 3-way handshaking ๊ณผ์ ์์ ํด๋ผ์ด์ธํธ๊ฐ ์๋ฒ๊ฐ ๋ณด๋ธ ACK+SYN์ ๋ฐ์ง ๋ชปํ๋ฉด? - ์๋ฒ ์ฌํ
```
ํด๋ผ์ด์ธํธ์์ ํน์  ์๊ฐ์ ๋๊ธฐํด๋ ์ ์ก์ด ์๋๋ ๊ฒฝ์ฐ ์์ฒญ SYN์ ์ฌ์ ์ก
```

#### ๐ก UDP์์ ์ ๋ขฐ๋๋ฅผ ๋ณด์ฅํ๋ ๋ฐฉ๋ฒ์ ์ค๋ชํด์ฃผ์ธ์.
```
๋ฐ์  ์์  IP ๋ฐ ํ๋กํ ์ฝ์์ ์ฒดํฌ์ฌ์ ๊ณ์ฐ
```

## [HTTP์ HTTPS](#http์-https-๋ต๋ณ)
#### ๐ก HTTP์ HTTPS๋ฅผ ์ค๋ชํด์ฃผ์ธ์
```
HTTP
HTTP(Hyper Text Transfer Protocol)๋ ์๋ฒ/ํด๋ผ์ด์ธํธ ๋ชจ๋ธ์ ๋ฐ๋ผ ๋ฐ์ดํฐ๋ฅผ ์ฃผ๊ณ  ๋ฐ๊ธฐ ์ํ ํ๋กํ ์ฝ์ด๋ค.

HTTPS
HyperText Transfer Protocol over Secure Socket Layer, HTTP over TLS, HTTP over SSL, HTTP Secure ๋ฑ์ผ๋ก ๋ถ๋ฆฌ๋ HTTPS๋ HTTP์ ๋ฐ์ดํฐ ์ํธํ๊ฐ ์ถ๊ฐ๋ ํ๋กํ ์ฝ์ด๋ค. HTTPS๋ HTTP์ ๋ค๋ฅด๊ฒ 433๋ฒ ํฌํธ๋ฅผ ์ฌ์ฉํ๋ฉฐ, ๋คํธ์ํฌ ์์์ ์ค๊ฐ์ ์ 3์๊ฐ ์ ๋ณด๋ฅผ ๋ณผ ์ ์๋๋ก ๊ณต๊ฐํค ์ํธํ๋ฅผ ์ง์
```
#### ๐ก HTTP์ ๋จ์ ์ ์ค๋ชํด์ฃผ์ธ์
```
HTTP๋ ์ํธํ๊ฐ ์ถ๊ฐ๋์ง ์์๊ธฐ ๋๋ฌธ์ ๋ณด์์ ์ทจ์ฝํ ๋ฐ๋ฉด, HTTPS๋ ์์ ํ๊ฒ ๋ฐ์ดํฐ๋ฅผ ์ฃผ๊ณ ๋ฐ์ ์ ์๋ค. ํ์ง๋ง HTTPS๋ฅผ ์ด์ฉํ๋ฉด ์ํธํ/๋ณตํธํ์ ๊ณผ์ ์ด ํ์ํ๊ธฐ ๋๋ฌธ์ HTTP๋ณด๋ค ์๋๊ฐ ๋๋ฆฌ๋ค.(์ค๋๋ ์๋ ๊ฑฐ์ ์ฐจ์ด๋ฅผ ๋ชป๋๋ ์ ๋์ด๋ค.) ๋ํ HTTPS๋ ์ธ์ฆ์๋ฅผ ๋ฐ๊ธํ๊ณ  ์ ์งํ๊ธฐ ์ํ ์ถ๊ฐ ๋น์ฉ์ด ๋ฐ์ํ๋ค.

๊ทธ๋ ๋ค๋ฉด ์ธ์  HTTP๋ฅผ ์ฐ๊ณ , ์ธ์  HTTPS๋ฅผ ์ฐ๋ ๊ฒ์ด ์ข๊ฒ ๋๊ฐ?

๊ฐ์ธ ์ ๋ณด์ ๊ฐ์ ๋ฏผ๊ฐํ ๋ฐ์ดํฐ๋ฅผ ์ฃผ๊ณ  ๋ฐ์์ผ ํ๋ค๋ฉด HTTPS๋ฅผ ์ด์ฉํด์ผ ํ์ง๋ง, ๋จ์ํ ์ ๋ณด ์กฐํ ๋ฑ๋ง์ ์ฒ๋ฆฌํ๊ณ  ์๋ค๋ฉด HTTP๋ฅผ ์ด์ฉํ๋ฉด ๋๋ค.
```

#### ๐ก HTTP 1.0+์ HTTP1.1์ HTTP2.0 ์ฐจ์ด์ ์ ๋ฌด์์ธ๊ฐ์?
```
HTTP 1.0
- TCP Connection๋น ํ๋์ URL๋ง fetchํ๋ฉฐ, ๋งค๋ฒ request/response๊ฐ ๋๋๋ฉด ์ฐ๊ฒฐ์ด ๋๊ธฐ๋ฏ๋ก ํ์ํ  ๋๋ง๋ค ๋ค์ ์ฐ๊ฒฐํด์ผํ๋ ๋จ์ ์ด ์์ด ์๋๊ฐ ํ์ ํ ๋๋ฆฌ๋ค.
URL์ ํฌ๊ธฐ๊ฐ ์๊ณ  ํ๋ฒ์ ๊ฐ์ ธ์ฌ ์ ์๋ ๋ฐ์ดํฐ์ ์์ด ์ ํ๋์ด ์๋ค.


HTTP 1.1
- HTTP์ ์ธํฐ๋ท์์ impact๋ฅผ ์ค์ด๊ณ  cache๋ฅผ ๋์ด ์ธํฐ๋ท ํ๋กํ ์ฝ ์ํ์ด ๋น ๋ฅด๊ฒ ๋  ์ ์๋๋ก ์ฑ๋ฅ์ ํฅ์ํ๊ณ  ์๋ค.
- multiple request์ ๋ํ ์ฒ๋ฆฌ๊ฐ ๊ฐ๋ฅํ๊ณ  request/response๊ฐ ํ์ดํ๋ผ์ธ ๋ฐฉ์์ผ๋ก ์งํ์ด ๊ฐ๋ฅํ๋ค.
- HTTP 1.1์ ๋ชจ๋  ์์ฒญ๊ณผ ์๋ต์ ๊ธฐ๋ณธ์ ์ผ๋ก Persistent Connection์ ์ง์
- ํ์ ์์ ๊ฒฝ์ฐ์๋ง(HTTP ์๋ต ์๋ฃ ํ TCP ์ฐ๊ฒฐ์ ๋์ด์ผํ๋ ๊ฒฝ์ฐ) Connection ํค๋๋ฅผ ์ฌ์ฉํ๋ค.

- HTTP 1.1์์๋ ํด๋ผ์ด์ธํธ์ ์๋ฒ๊ฐ์ ์์ฒญ๊ณผ ์๋ต ํจ์จ์ฑ์ ๊ฐ์ ํ๊ธฐ ์ํด HTTP Pipelining์ด ๋ฑ์ฅํ์๋ค.
```
#### ๐ก ๋น๋์นญํค ๋๋ ๊ณต๊ฐํค ์ํธํ ๋ฐฉ์์ ๋ฌด์์ธ๊ฐ์?
```
A๋ ๊ณต๊ฐํค(Public key)์ ๊ฐ์ธํค(Private key)๋ฅผ ์์ฑํ๋ค.
๊ณต๊ฐํค ์ํธํ: A์ ๊ณต๊ฐํค๋ฅผ ์ด์ฉํ์ฌ ์ํธํ๋ ๋ฐ์ดํฐ๋ A์ ๊ฐ์ธํค๋ก๋ง ๋ณตํธํ๊ฐ ๊ฐ๋ฅํ๋ค.
๊ฐ์ธํค ์ํธํ: A์ ๊ฐ์ธํค๋ฅผ ์ด์ฉํ์ฌ ์ํธํ๋ ๋ฐ์ดํฐ๋ A์ ๊ณต๊ฐํค๋ก๋ง ๋ณตํธํ๊ฐ ๊ฐ๋ฅํ๋ค.
B๋ A์ ๊ณต๊ฐํค๋ฅผ ์กฐํํ๊ณ , A์ ๊ณต๊ฐํค๋ฅผ ์ด์ฉํ์ฌ ๋ฐ์ดํฐ๋ฅผ ์ํธํํ ํ ์ ์กํ๋ค.
A๋ ๊ฐ์ธํค๋ก ์ํธํ๋ ๋ฐ์ดํฐ๋ฅผ ๋ณตํธํํ๋ค.
```

#### ๐ก HTTP REQUEST ๋ฐฉ์ ์ค GET๊ณผ POST์ ์ฐจ์ด์ ์ค๋ชํด์ฃผ์ธ์.
```
์ฌ์ฉ๋ชฉ์  : GET์ ์๋ฒ์ ๋ฆฌ์์ค์์ ๋ฐ์ดํฐ๋ฅผ ์์ฒญํ  ๋, POST๋ ์๋ฒ์ ๋ฆฌ์์ค๋ฅผ ์๋ก ์์ฑํ๊ฑฐ๋ ์๋ฐ์ดํธํ  ๋ ์ฌ์ฉํ๋ค. 

์์ฒญ์ body ์ ๋ฌด : GET ์ URL ํ๋ผ๋ฏธํฐ์ ์์ฒญํ๋ ๋ฐ์ดํฐ๋ฅผ ๋ด์ ๋ณด๋ด๊ธฐ ๋๋ฌธ์ HTTP ๋ฉ์์ง์ body๊ฐ ์๋ค. POST ๋ body ์ ๋ฐ์ดํฐ๋ฅผ ๋ด์ ๋ณด๋ด๊ธฐ ๋๋ฌธ์ ๋น์ฐํ HTTP ๋ฉ์์ง์ body๊ฐ ์กด์ฌํ๋ค.

๋ฉฑ๋ฑ์ฑ (idempotent) : GET ์์ฒญ์ ๋ฉฑ๋ฑ์ด๋ฉฐ, POST๋ ๋ฉฑ๋ฑ์ด ์๋๋ค.
```

#### ๐ก GET, POST๋ฅผ ์ ์ธํ๊ณ  ๋ค๋ฅธ ๋ฐฉ์๋ค์ ์ค๋ชํด์ฃผ์ธ์.
```
OPTION : ํต์ ๊ณผ ๊ด๋ จ๋ ์ ํ์ฌํญ๋ค์ ๋ํ ์ ๋ณด๋ฅผ ์๊ตฌํ๋ ๊ฒฝ์ฐ
PUT : Request ๋ฉ์์ง์ ํฌํจ๋์ด ์๋ data๋ฅผ ์ง์ ํ Request-URI๋ก ์ ์ฅํ๊ธฐ ์ํจ
DELETE : ํน์  resource๋ฅผ ์ง์ฐ๊ธฐ ์ํจ
TRACE : ์ต์ข destination๊น์ง์ Loopback์ ํ์คํธํ๊ธฐ ์ํจ
```
#### ๐ก ์กฐํํ๊ธฐ ์ํ ์ฉ๋ POST๊ฐ ์๋ GET ๋ฐฉ์์ ์ฌ์ฉํ๋ ์ด์ ?  
```
๋ฉฑ๋ฑ์ฑ ๋๋ฌธ์
```
#### ๐ก ํ๋ ์น ์์๋ ๋น์ฐ๊ฒฐ์ฑ์ ํด๊ฒฐ๋ฐฉ๋ฒ์ ์ค๋ชํด์ฃผ์ธ์. - ์๋ฒ ์ฌํ
```
์ฟ ํค, ์ธ์, ํ ํฐ์ ์ฌ์ฉ
```

## [๋ก๋๋ฐธ๋ฐ์](#๋ก๋๋ฐธ๋ฐ์-๋ต๋ณ) - ์๋ฒ ๊ฐ๋ฐ์๋ง ๋ต๋ณํ  ๊ฒ
#### ๐ก ๋ก๋ ๋ฐธ๋ฐ์ฑ์ ์ค๋ชํด์ฃผ์ธ์.  
<<<<<<< HEAD
```
ํ๋์ ์ธํฐ๋ท ์๋น์ค๊ฐ ๋ฐ์ํ๋ ํธ๋ํฝ์ด ๋ง์ ๋ ์ฌ๋ฌ ๋์ ์๋ฒ๊ฐ ๋ถ์ฐ์ฒ๋ฆฌํ์ฌ ์๋ฒ์ ๋ก๋์จ ์ฆ๊ฐ, ๋ถํ๋, ์๋์ ํ ๋ฑ์ ๊ณ ๋ คํ์ฌ ์ ์ ํ ๋ถ์ฐ์ฒ๋ฆฌํ์ฌ ํด๊ฒฐํด์ฃผ๋ ์๋น์ค์๋๋ค.
```
#### ๐ก L4 ๋ก๋ ๋ฐธ๋ฐ์ฑ๊ณผ L7 ๋ก๋ ๋ฐธ๋ฐ์ฑ์ ๋ํด ์ค๋ชํ๊ณ , ์ฐจ์ด๋ฅผ ๋งํด๋ณด์ธ์
```
L4 ๋ก๋ ๋ฐธ๋ฐ์ฑ - ๋คํธ์ํฌ ๊ณ์ธต์์ ๋์ - NLB

ํ๋ฐ์ฑ ์ฒ๋ฆฌ ์ด๋น ์๋ฐฑ๋ง๊ฐ ์ฒ๋ฆฌ ๊ฐ๋ฅ
๋ก๋ ๋ฐธ๋ฐ์์ ๋ํ ๊ณ ์  IP ์ฃผ์ ์ง์

L7 ๋ก๋ ๋ฐธ๋ฐ์ฑ - ์ดํ๋ฆฌ์ผ์ด์ ๊ณ์ธต์์ ๋์ - ALB 
 
path-based(๊ฒฝ๋ก ๊ธฐ๋ฐ) ๋ผ์ฐํ์ด ์ง์๋๋ค
HTTP ํค๋์ ํธ์คํธ ํ๋๋ฅผ ๊ธฐ๋ฐ์ผ๋ก ๋ผ์ฐํ์ ์ง์
``` 
#### ๐ก ๊ฒ์ดํธ์จ์ด๋?  
```
ํ ๋คํธ์ํฌ(segment)์์ ๋ค๋ฅธ ๋คํธ์ํฌ๋ก ์ด๋ํ๊ธฐ ์ํ์ฌ ๊ฑฐ์ณ์ผ ํ๋ ์ง์ ์๋๋ค.

๊ฒ์ดํธ์จ์ด(Gateway)๋ ์๋ก ๋ค๋ฅธ ๋คํธ์ํฌ๋ฅผ ์ฐ๊ฒฐํด์ค๋๋ค. ์๋ก ๋ค๋ฅธ ๋คํธ์ํฌ์ ํ๋กํ ์ฝ์ด ๋ค๋ฅผ ๊ฒฝ์ฐ์ ์ค์ฌ ์ญํ ์ ํด์ค๋ค๊ณ  ๋ณด๋ฉด ๋๋ค.
```
#### ๐ก ์๋ฒ์ ํธ๋ํฝ์ด ์ฃผ์ด์ก์ ๋ ์ด๋ป๊ฒ ์๋ต์๋๋ฅผ ๊ฐ์ ํ  ์ ์๋๊ฐ?  
```
1. ์บ์ ํ๋ก์ ์๋ฒ๋ฅผ ๊ตฌ์ฑํ์ฌ ์์ฃผ ์์ฒญํ๋ ๋ฐ์ดํฐ์ ๋ํด์ ๊ตฌ์ถ (Nginx Reverse Proxy Server)
2. ์ดํ๋ฆฌ์ผ์ด์ ๊ฐ์  ์๋ ํ์ฐ์ ์ํด์ DB ์ ์ ์๋ ๊ฐ์ (Redis ์ฌ์ฉ ๋ฑ)
```
#### ๐ก ํ๋ผ์ด๋น ์๋ธ๋ท๊ณผ ํผ๋ธ๋ฆญ ์๋ธ๋ท์ ์ฐจ์ด
```
VPC๋ณด๋ค ์์ ๋จ์์๊ฐ ์๋ธ๋ท์ด๊ณ  ์ฐ์ ์์๋ฅผ ๋๊ฒ ๊ฐ์ง๊ฒ ๋๋ค

์ธํฐ๋ท๊ณผ ์ฐ๊ฒฐ๋์ด ์๋ ์๋ธ๋ท์ ํผ๋ธ๋ฆญ ์๋ธ๋ท์ด๊ณ  ์ธํฐ๋ท๊ณผ ์ฐ๊ฒฐ๋์ด ์์ง ์์ ์๋ธ๋ท์ ํ๋ผ์ด๋น ์๋ธ๋ท์ด๋ผ๊ณ  ํ๋ค
```

## 01-2. Web of Network Overview
## [WEB](#web-๋ต๋ณ)
#### ๐ก url๊ณผ uri์ ๋ํด ๊ฐ๊ฐ ์ค๋ชํด์ฃผ์ธ์
```
URI๋ ํน์  ๋ฆฌ์์ค๋ฅผ ์๋ณํ๋ ํตํฉ ์์ ์๋ณ์(Uniform Resource Identifier)๋ฅผ ์๋ฏธํ๋ค. ์น ๊ธฐ์ ์์ ์ฌ์ฉํ๋ ๋ผ๋ฆฌ์  ๋๋ ๋ฌผ๋ฆฌ์  ๋ฆฌ์์ค๋ฅผ ์๋ณํ๋ ๊ณ ์ ํ ๋ฌธ์์ด ์ํ์ค๋ค.

URL์ ํํ ์น ์ฃผ์๋ผ๊ณ ๋ ํ๋ฉฐ, ์ปดํจํฐ ๋คํธ์ํฌ ์์์ ๋ฆฌ์์ค๊ฐ ์ด๋ ์๋์ง ์๋ ค์ฃผ๊ธฐ ์ํ ๊ท์ฝ์ด๋ค. URI์ ์๋ธ์์ด๋ค.

ํ๋์  ๊ด์ ์์๋ ๋์ ํฌ๊ฒ ์ฐจ์ด ์ ์ด ์๋ค๊ณ  ๋ณด๋ฉด ๋๋ค.
```

#### ๐ก ๋ธ๋ผ์ฐ์ ์ "www.google.com" ์๋ ฅํ๋ฉด ์ด๋ค์ผ์ด ์ผ์ด๋ ๊น์?  
```
1. ์ผ๋จ, ์น ๋ธ๋ผ์ฐ์ ์ URL์ ์๋ ฅํ๊ณ  Enter๋ฅผ ํด๋ฆญํฉ๋๋ค.
2. ๊ทธ๋ผ ๋ฐ๋ก URL์ ์ฃผ์๋ก ์ด๋ ์น ๋ธ๋ผ์ฐ์ ๊ฐ ์๋ ฅํ URL์ ๋ถ์ํ๋ฉฐ ์ผ์ ํ๊ธฐ ์์ํฉ๋๋ค.
3. URL์ ๋ถ์ํ ๋ค์,
4. DNS( Domain Name Server )์ ๋ด๊ฐ ์ ๊ทผํ๋ ค๋ name ์ฃผ์์ IP ์ฃผ์๋ฅผ ์์ฒญํ๋ค.
5. IP์ฃผ์๋ฅผ ๋ฐ์ ๋ค์, ARP๋ฅผ ํตํด ์ค์ง์ ์ผ๋ก ๋ด๊ฐ ์ ๊ทผํด์ผํ  IP์ฃผ์๋ฅผ ํ ๋น๋ฐ์ ๋์์ MAC ์ฃผ์๋ฅผ ์ถ์ ํ๋ค.
6. ๋์๊ณผ TCP ํต์ ์ ํตํด Socket์ ์ฐ๋ค.
7. HTTPS => TLS(Seucure Sockets Layer)๊ณผ์  ์ถ๊ฐ
8. HTTP ํ๋กํ ์ฝ ์์ฒญ
9. HTTP์ ์๋ต
10. ์น ๋ธ๋ผ์ฐ์ ์ ๊ทธ๋ฆผ ๊ทธ๋ฆฌ๊ธฐ
```
#### ๐ก RESTful API๋ ๋ฌด์์ธ๊ฐ์? 
```
1.์์ : URI
2.ํ์ : Method
3.ํํ : Client์ ๋ํ ์ ์ ํ JSON, XL, TEXT, RSS ๋ฑ์ ์ฌ๋ฌ Representation
์ผ๋ก ๊ตฌ์ฑ๋ API ํํ
``` 
#### ๐ก Ajax๋ ๋ฌด์์ธ๊ฐ์?  
```
JavaScript๋ฅผ ์ฌ์ฉํ ๋น๋๊ธฐ ํต์ , ํด๋ผ์ด์ธํธ์ ์๋ฒ๊ฐ์ XML ๋ฐ์ดํฐ๋ฅผ ์ฃผ๊ณ ๋ฐ๋ ๊ธฐ์ 
```
#### ๐ก Ajax์ ์ฅ์ ๊ณผ ๋จ์ ์ ๋ฌด์์ธ๊ฐ์? - ์น ์ฌํ  
```
1. AJAX์ ์ฅ์ 
- ์นํ์ด์ง์ ์๋ํฅ์
- ์๋ฒ์ ์ฒ๋ฆฌ๊ฐ ์๋ฃ๋  ๋๊น์ง ๊ธฐ๋ค๋ฆฌ์ง ์๊ณ  ์ฒ๋ฆฌ๊ฐ ๊ฐ๋ฅํ๋ค.
- ์๋ฒ์์ Data๋ง ์ ์กํ๋ฉด ๋๋ฏ๋ก ์ ์ฒด์ ์ธ ์ฝ๋ฉ์ ์์ด ์ค์ด๋ ๋ค.
- ๊ธฐ์กด ์น์์๋ ๋ถ๊ฐ๋ฅํ๋ ๋ค์ํ UI๋ฅผ ๊ฐ๋ฅํ๊ฒ ํด์ค๋ค.

2. AJAX์ ๋จ์ 
- ํ์คํ ๋ฆฌ ๊ด๋ฆฌ๊ฐ ๋์ง ์๋๋ค.
- ํ์ด์ง ์ด๋์๋ ํต์ ์ผ๋ก ์ธํ ๋ณด์์์ ๋ฌธ์ ๊ฐ ์๋ค.
- ์ฐ์์ผ๋ก ๋ฐ์ดํฐ๋ฅผ ์์ฒญํ๋ฉด ์๋ฒ ๋ถํ๊ฐ ์ฆ๊ฐํ  ์ ์๋ค.
- XMLHttpRequest๋ฅผ ํตํด ํต์ ํ๋ ๊ฒฝ์ฐ, ์ฌ์ฉ์์๊ฒ ์๋ฌด๋ฐ ์งํ ์ ๋ณด๊ฐ ์ฃผ์ด์ง์ง ์๋๋ค. 
- AJAX๋ฅผ ์ธ ์ ์๋ ๋ธ๋ผ์ฐ์ ์ ๋ํ ๋ฌธ์  ์ด์๊ฐ ์๋ค.
- HTTP ํด๋ผ์ด์ธํธ์ ๊ธฐ๋ฅ์ด ํ์ ๋์ด ์๋ค.
- ์ง์ํ๋ Charset์ด ํ์ ๋์ด ์๋ค.
- Script๋ก ์์ฑ๋๋ฏ๋ก ๋๋ฒ๊น์ด ์ฉ์ดํ์ง ์๋ค.
- ๋์ผ-์ถ์ฒ ์ ์ฑ์ผ๋ก ์ธํ์ฌ ๋ค๋ฅธ ๋๋ฉ์ธ๊ณผ๋ ํต์ ์ด ๋ถ๊ฐ๋ฅํ๋ค. 
```

#### ๐ก CORS๋ ๋ฌด์์ธ๊ฐ์?  
```
๊ต์ฐจ ์ถ์ฒ ๋ฆฌ์์ค ๊ณต์ (Cross-Origin Resource Sharing, CORS)๋ ์ถ๊ฐ HTTP ํค๋๋ฅผ ์ฌ์ฉํ์ฌ, ํ ์ถ์ฒ์์ ์คํ ์ค์ธ ์น ์ ํ๋ฆฌ์ผ์ด์์ด ๋ค๋ฅธ ์ถ์ฒ์ ์ ํํ ์์์ ์ ๊ทผํ  ์ ์๋ ๊ถํ์ ๋ถ์ฌํ๋๋ก ๋ธ๋ผ์ฐ์ ์ ์๋ ค์ฃผ๋ ์ฒด์ 
```
#### ๐ก CORS preflight๋ ๋ฌด์์ธ๊ฐ์? - ์น ์ฌํ 
```
๊ธฐ๋ณธ์ ์ผ๋ก ๋ธ๋ผ์ฐ์ ๋ cross-origin ์์ฒญ์ ์ ์กํ๊ธฐ ์ ์ OPTIONS ๋ฉ์๋๋ก preflight๋ฅผ ์ ์กํ๋ค.

์ด๋ Response๋ก Access-Control-Allow-Origin๊ณผ Access-Control-Allow-Methods๊ฐ ๋์ด์ค๋๋ฐ ์ด๋ ์๋ฒ์์ ์ด๋ค origin๊ณผ ์ด๋ค method๋ฅผ ํ์ฉํ๋์ง ๋ธ๋ผ์ฐ์ ์๊ฒ ์๋ ค์ฃผ๋ ์ญํ ์ ํ๋ค.

๋ธ๋ผ์ฐ์ ๊ฐ ๊ฒฐ๊ณผ๋ฅผ ์ฑ๊ณต์ ์ผ๋ก ํ์ธํ๊ณ  ๋๋ฉด cross-origin ์์ฒญ์ ๋ณด๋ด์ ๊ทธ ์ดํ ๊ณผ์ ์ ์งํ
```
#### ๐ก ์์ผ์ด๋ ๋ฌด์์ธ๊ฐ์?  
```
๋ ํธ์คํธ๋ฅผ ์ฐ๊ฒฐํด์ฃผ๋ ๋๊ตฌ๋ก์ ์ธํฐํ์ด์ค ์ญํ ์ ํจ

Socket ํต์ 

์๋ฒ์ ํด๋ผ์ด์ธํธ๊ฐ ํน์  ํฌํธ๋ฅผ ํตํด ์๋ฐฉํฅ ํต์ ์ ํ๋ ๋ฐฉ์
Server์ Client๋ฅผ ํตํด์ ๊ณ์ ์ฐ๊ฒฐ์ ์ ์งํ๋ ์๋ฐฉํฅ ํต์ 
์ค์๊ฐ Streaming / ์จ๋ผ์ธ ๊ฒ์

```
#### ๐ก DOM๊ณผ ๊ฐ์DOM - ์น ์ฌํ
```
DOM

์ฒซ์งธ, ๋ธ๋ผ์ฐ์ ๋ htmlํ๊ทธ๋ฅผ ํ์ฑ ํ์ฌ ๋ ํธ๋ฆฌ๋ฅผ ๊ตฌ์ฑํ๋ค.

๋์์ ๋ธ๋ผ์ฐ์ ๋ ์คํ์ผ์ํธ์์ css๋ฅผ ํ์ฑ ํ์ฌ ์คํ์ผ ๊ท์น๋ค์ ๋ง๋ค์ด๋ธ๋ค.

๋์งธ, ์์์ ์ธ๊ธํ ๋ ํธ๋ฆฌ์ ์คํ์ผ ๊ท์น ๋ ๊ฐ์ง๊ฐ ํฉ์ณ์ ธ์ ๋ ๋ ํธ๋ฆฌ๋ฅผ ๋ง๋ค์ด๋ธ๋ค.

๊ฐ์ ๋(Vitual DOM)

ํ๋ฉด์ ๋ณํ๊ฐ ์์ ๋๋ง๋ค ์ค์๊ฐ์ผ๋ก ๋ ํธ๋ฆฌ๋ฅผ ์์ ํ์ง ์๊ณ  ๋ณ๊ฒฝ์ฌํญ์ด ๋ชจ๋ ๋ฐ์๋ ๊ฐ์ ๋์ ๋ง๋ค์ด๋ธ๋ค. ๊ทธ ํ ๊ฐ์ ๋์ ์ด์ฉํด ํ ๋ฒ๋ง ๋์์ ์ ํ๊ฒ ๋๊ณ  ์ด๋ ํ ๋ฒ๋ง ๋ ๋ ํธ๋ฆฌ๋ฅผ ๋ง๋ค์ด๋ด๊ฒ ๋๋ค. ๋ธ๋ผ์ฐ์ ๋ ํ๋ฒ๋ง ๋ ๋๋ง์ ํ๊ฒ ๋จ์ผ๋ก์จ ๋ถํ์ํ ๋ ๋๋ง ํ์๋ฅผ ์ค์ผ ์ ์๊ฒ ๋๋ ๊ฒ

```  
#### ๐ก OAuth๋ ๋ฌด์์ธ๊ฐ์?  
```
OAuth๋ ์ธ์ฆ์ ์ํ ์คํ ์คํ ๋๋ ํ๋กํ ์ฝ๋ก, ์ฌ์ฉ์๊ฐ Facebook์ด๋ ํธ์ํฐ ๊ฐ์ ์ธํฐ๋ท ์๋น์ค์ ๊ธฐ๋ฅ์ ๋ค๋ฅธ ์ ํ๋ฆฌ์ผ์ด์(๋ฐ์คํฌํฑ, ์น, ๋ชจ๋ฐ์ผ ๋ฑ)์์๋ ์ฌ์ฉ ๊ฐ๋ฅํ๊ฒ ํ ๊ฒ

API ์ ๊ทผ ์์(API Access Delegation)์ ํตํด ์ธ์ฆ์ ์งํ
```
#### ๐ก SPA   
```
- ์น ์ฌ์ดํธ์ ์ ์ฒด ํ์ด์ง๋ฅผ ํ๋์ ํ์ด์ง์ ๋ด์ ๋์ ์ผ๋ก ํ๋ฉด์ ๋ฐ๊ฟ๊ฐ๋ฉฐ ํํํ๋ ๊ฒ์ด SPA
- ๋ญ๊ฐ๋ฅผ ํด๋ฆญํ๊ฑฐ๋ ์คํฌ๋กคํ๋ฉด, ์ํธ์์ฉํ๊ธฐ ์ํ ์ต์ํ์ ์์๋ง ๋ณ๊ฒฝ์ด ๋ฐ์
- ํ์ด์ง ๋ณ๊ฒฝ์ด ์ผ์ด๋๋ค๊ณ  ๋ณด์ฌ์ง๋ ๊ฒ ๋ํ ์ต์ด ๋ก๋๋ ์๋ฐ์คํฌ๋ฆฝํธ๋ฅผ ํตํด ๋ฏธ๋ฆฌ ๋ธ๋ผ์ฐ์ ์ ์ฌ๋ผ๊ฐ ํํ๋ฆฟ๋ง ๊ต์ฒด๋๋ ๊ฒ
```

## [cookie์ session](#cookie์-session-๋ต๋ณ)
#### ๐ก cookie์ session์ ๋ํด ์ค๋ชํด์ฃผ์ธ์  
```
์ฟ ํค

- ์น ์๋ฒ๊ฐ ๋ธ๋ผ์ฐ์ ์๊ฒ ์ง์ํ์ฌ ์ฌ์ฉ์์ ๋ก์ปฌ ์ปดํจํฐ์ 
 ํ์ผ ๋๋ ๋ฉ๋ชจ๋ฆฌ์ ์ ์ฅํ๋ ์์ ๊ธฐ๋ก ์ ๋ณด ํ์ผ
- ํ์ผ์ ๋ด๊ธด ์ ๋ณด๋ ์ธํฐ๋ท ์ฌ์ฉ์๊ฐ ๊ฐ์ ์น์ฌ์ดํธ๋ฅผ ๋ฐฉ๋ฌธํ  ๋๋ง๋ค ์ฝํ๊ณ  ์์๋ก ์๋ก์ด ์ ๋ณด๋ก ๋ฐ๋

์ธ์

- HTTP Session id๋ฅผ ์๋ณ์๋ก ๊ตฌ๋ณํ์ฌ ๋ฐ์ดํฐ๋ฅผ ์ฌ์ฉ์์ ๋ธ๋ผ์ฐ์ ์ ์ฟ ํคํํ๊ฐ ์๋ ์ ์ํ ์๋ฒ DB์ ์ ๋ณด๋ฅผ ์ ์ฅ
- ํด๋ผ์ด์ธํธ๋ HTTP Session id๋ฅผ ์ฟ ํค๋ก ๋ฉ๋ชจ๋ฆฌ ์ ์ฅ๋ ํํ ์์ง
- ๋ฉ๋ชจ๋ฆฌ์ ์ ์ฅํ๊ธฐ ๋๋ฌธ์ ๋ธ๋ผ์ฐ์ ๊ฐ ์ข๋ฃ๋๋ฉด ์ฌ๋ผ์ง.

```
#### ๐ก Session ๋์ ์์๋ฅผ ์ค๋ชํด์ฃผ์ธ์.  
```
- ํด๋ผ์ด์ธํธ๊ฐ ์๋ฒ์ Resource๋ฅผ ์์ฒญ

- ์๋ฒ์์๋ HTTP Request๋ฅผ ํตํด ์ฟ ํค์์ Session id๋ฅผ ํ์ธ์ ํ ํ์ ์์ผ๋ฉด Set-Cookie๋ฅผ ํตํด ์๋ก ๋ฐํํ Session-id ์ ์ก

- ํด๋ผ์ด์ธํธ๋ HTTP Request ํค๋์ Session id๋ฅผ ํฌํจํ์ฌ ์ํ๋ Resource๋ฅผ ์์ฒญ

- ์๋ฒ๋ Session id๋ฅผ ํตํด ํด๋น ์ธ์์ ์ฐพ์ ํด๋ผ์ด์ธํธ ์ํ ์ ๋ณด๋ฅผ ์ ์งํ๋ฉฐ ์ ์ ํ ์๋ต
```

#### ๐ก cookie๋ฅผ ์ฐ๋ ์ด์ ๋ฅผ ์ค๋ชํด์ฃผ์ธ์  
```
์ ๋ณด๋ฅผ ์ ์งํ  ์ ์๋ Connectionless, Stateless์ ์ฑ๊ฒฉ์ ๊ฐ์ง HTTP์ ๋จ์ ์ ํด๊ฒฐํ๊ธฐ ์ํด ์ฟ ํค๋ผ๋ ๊ฐ๋์ด ๋์
```

#### ๐ก ์ธ์ ์ธ์ฆ๋ฐฉ์ ๋จ์   
```
load-balancing/์์คํ ํจ์จ์ฑ์์ handlingํ๊ธฐ ์ด๋ ค์
์ธ์ ์ ์ฅ ์ฅ์น๊ฐ ๋ถ์กฑํ ์์คํ์๋ ์ ํฉํ์ง ์์
```
#### ๐ก ํ ํฐ ์ธ์ฆ๋ฐฉ์
```
1. ์ธ์ฆ๋ฐ์ ์ฌ์ฉ์๋ค์๊ฒ ํ ํฐ์ ๋ฐ๊ธํ๊ณ , ์๋ฒ์ ์์ฒญ์ ํ  ๋ ํค๋์ ํ ํฐ์ ํจ๊ป ๋ณด๋ด๋๋ก ํ์ฌ ์ ํจ์ฑ ๊ฒ์ฌ ์งํ
2. ์์คํ์์๋ ๋์ด์ ์ฌ์ฉ์์ ์ธ์ฆ ์ ๋ณด๋ฅผ ์๋ฒ๋ ์ธ์์ ์ ์งํ์ง ์๊ณ  ํด๋ผ์ด์ธํธ ์ธก์์ ๋ค์ด์ค๋ ์์ฒญ๋ง์ผ๋ก ์์์ ์ฒ๋ฆฌ 
์๋ฒ ๊ธฐ๋ฐ์ ์ธ์ฆ ์์คํ๊ณผ ๋ฌ๋ฆฌ ์ํ๋ฅผ ์ ์งํ์ง ์์ผ๋ฏ๋ก Statelessํ ๊ตฌ์กฐ๋ฅผ ์ ์ง
```

#### ๐ก JWT   
```
Json ํฌ๋งท์ ์ด์ฉํ์ฌ ์ฌ์ฉ์์ ๋ํ ์์ฑ์ ์ ์ฅํ๋ Claim ๊ธฐ๋ฐ์ Web Token์ด๋ค. JWT๋ ํ ํฐ ์์ฒด๋ฅผ ์ ๋ณด๋ก ์ฌ์ฉํ๋ Self-Contained ๋ฐฉ์์ผ๋ก ์ ๋ณด๋ฅผ ์์ ํ๊ฒ ์ ๋ฌ

JWT๋ Header, Payload, Signature์ 3 ๋ถ๋ถ์ผ๋ก ์ด๋ฃจ์ด์ง๋ฉฐ, Json ํํ์ธ ๊ฐ ๋ถ๋ถ์ Base64๋ก ์ธ์ฝ๋ฉ ๋์ด ํํ๋๋ค. ๋ํ ๊ฐ๊ฐ์ ๋ถ๋ถ์ ์ด์ด ์ฃผ๊ธฐ ์ํด . ๊ตฌ๋ถ์๋ฅผ ์ฌ์ฉํ์ฌ ๊ตฌ๋ถํ๋ค. ์ถ๊ฐ๋ก Base64๋ ์ํธํ๋ ๋ฌธ์์ด์ด ์๋๊ณ , ๊ฐ์ ๋ฌธ์์ด์ ๋ํด ํญ์ ๊ฐ์ ์ธ์ฝ๋ฉ ๋ฌธ์์ด์ ๋ฐํ

```
![jwt1](./jwt1.png)

![jwt2](,/jwt2.png)
#### ๐ก ํ ํฐ ์ธ์ฆ๋ฐฉ์ ๋จ์   
```
Self-contained: ํ ํฐ ์์ฒด์ ์ ๋ณด๋ฅผ ๋ด๊ณ  ์์ผ๋ฏ๋ก ์๋ ์ ๊ฒ์ด ๋  ์ ์๋ค.

ํ ํฐ ๊ธธ์ด: ํ ํฐ์ ํ์ด๋ก๋(Payload)์ 3์ข๋ฅ์ ํด๋ ์์ ์ ์ฅํ๊ธฐ ๋๋ฌธ์, ์ ๋ณด๊ฐ ๋ง์์ง์๋ก ํ ํฐ์ ๊ธธ์ด๊ฐ ๋์ด๋ ๋คํธ์ํฌ์ ๋ถํ๋ฅผ ์ค ์ ์๋ค.

Payload ์ธ์ฝ๋ฉ: ํ์ด๋ก๋(Payload) ์์ฒด๋ ์ํธํ ๋ ๊ฒ์ด ์๋๋ผ, BASE64๋ก ์ธ์ฝ๋ฉ ๋ ๊ฒ์ด๋ค. ์ค๊ฐ์ Payload๋ฅผ ํ์ทจํ์ฌ ๋์ฝ๋ฉํ๋ฉด ๋ฐ์ดํฐ๋ฅผ ๋ณผ ์ ์์ผ๋ฏ๋ก, JWE๋ก ์ํธํํ๊ฑฐ๋ Payload์ ์ค์ ๋ฐ์ดํฐ๋ฅผ ๋ฃ์ง ์์์ผ ํ๋ค.

Stateless: JWT๋ ์ํ๋ฅผ ์ ์ฅํ์ง ์๊ธฐ ๋๋ฌธ์ ํ๋ฒ ๋ง๋ค์ด์ง๋ฉด ์ ์ด๊ฐ ๋ถ๊ฐ๋ฅํ๋ค. ์ฆ, ํ ํฐ์ ์์๋ก ์ญ์ ํ๋ ๊ฒ์ด ๋ถ๊ฐ๋ฅํ๋ฏ๋ก ํ ํฐ ๋ง๋ฃ ์๊ฐ์ ๊ผญ ๋ฃ์ด์ฃผ์ด์ผ ํ๋ค.

Tore Token: ํ ํฐ์ ํด๋ผ์ด์ธํธ ์ธก์์ ๊ด๋ฆฌํด์ผ ํ๊ธฐ ๋๋ฌธ์, ํ ํฐ์ ์ ์ฅํด์ผ ํ๋ค.

```
#### ๐ก ์ฟ ํค ์ธ์ฆ๋ฐฉ์ ํด๊ฒฐ๋ฐฉ์  
```
JWT๋ฅผ ์ฌ์ฉํด์ ์ธ์ฆ
```
=======
#### ๐ก L4 ๋ก๋ ๋ฐธ๋ฐ์ฑ๊ณผ L7 ๋ก๋ ๋ฐธ๋ฐ์ฑ์ ๋ํด ์ค๋ชํ๊ณ , ์ฐจ์ด๋ฅผ ๋งํด๋ณด์ธ์  
#### ๐ก ๊ฒ์ดํธ์จ์ด๋?  
#### ๐ก ์๋ฒ์ ํธ๋ํฝ์ด ์ฃผ์ด์ก์ ๋ ์ด๋ป๊ฒ ์๋ต์๋๋ฅผ ๊ฐ์ ํ  ์ ์๋๊ฐ?  
#### ๐ก ํ๋ผ์ด๋น ์๋ธ๋ท๊ณผ ํผ๋ธ๋ฆญ ์๋ธ๋ท์ ์ฐจ์ด

## 01-2. Web of Network Overview
## [WEB](#web-๋ต๋ณ)
#### ๐ก url๊ณผ uri์ ๋ํด ๊ฐ๊ฐ ์ค๋ชํด์ฃผ์ธ์  
#### ๐ก ๋ธ๋ผ์ฐ์ ์ "www.google.com" ์๋ ฅํ๋ฉด ์ด๋ค์ผ์ด ์ผ์ด๋ ๊น์?  
#### ๐ก RESTful API๋ ๋ฌด์์ธ๊ฐ์?  
#### ๐ก Ajax๋ ๋ฌด์์ธ๊ฐ์?  
#### ๐ก Ajax์ ์ฅ์ ๊ณผ ๋จ์ ์ ๋ฌด์์ธ๊ฐ์? - ์น ์ฌํ  
#### ๐ก CORS๋ ๋ฌด์์ธ๊ฐ์?  
#### ๐ก CORS preflight๋ ๋ฌด์์ธ๊ฐ์? - ์น ์ฌํ 
#### ๐ก ์์ผ์ด๋ ๋ฌด์์ธ๊ฐ์?  
#### ๐ก DOM๊ณผ ๊ฐ์DOM - ์น ์ฌํ  
#### ๐ก OAuth๋ ๋ฌด์์ธ๊ฐ์?  
#### ๐ก SPA   

## [cookie์ session](#cookie์-session-๋ต๋ณ)
#### ๐ก cookie์ session์ ๋ํด ์ค๋ชํด์ฃผ์ธ์  
#### ๐ก Session ๋์ ์์๋ฅผ ์ค๋ชํด์ฃผ์ธ์.  
#### ๐ก cookie๋ฅผ ์ฐ๋ ์ด์ ๋ฅผ ์ค๋ชํด์ฃผ์ธ์  
#### ๐ก ์ธ์ ์ธ์ฆ๋ฐฉ์ ๋จ์   
#### ๐ก ํ ํฐ ์ธ์ฆ๋ฐฉ์
#### ๐ก JWT   
#### ๐ก ํ ํฐ ์ธ์ฆ๋ฐฉ์ ๋จ์   
#### ๐ก ์ฟ ํค ์ธ์ฆ๋ฐฉ์ ํด๊ฒฐ๋ฐฉ์  

refered by https://github.com/SSAFY-CS-STUDY/
>>>>>>> 9e5c616fd0fc2dd197862be9378a9717e4d3ae03
