## RDBMS / NoSQL

#### ๐ก๊ด๊ณํ ๋ฐ์ดํฐ๋ฒ ์ด์ค์ ํน์ง

- ๊ด๊ณํ ๋ฐ์ดํฐ๋ฒ ์ด์ค๋ ๋ฐ์ดํฐ์ ๋ถ๋ฅ, ์ ๋ ฌ, ํ์ ์๋๊ฐ ๋น ๋ฆ๋๋ค. ๋ํ, ๋ฐ์ดํฐ์ ๋ฌด๊ฒฐ์ฑ์ ๋ณด์ฅํ๋ค๋ ํน์ง์ด ์์ต๋๋ค.

<br>

#### ๐ก๋ฌด๊ฒฐ์ฑ ์ ์ฝ์กฐ๊ฑด์ด๋ ๋ฌด์์ธ๊ฐ?

- ๋ฐ์ดํฐ๋ฒ ์ด์ค์ ์ ์ฅ๋ ๋ฐ์ดํฐ์ ๋ฌด๊ฒฐ์ฑ์ ๋ณด์ฅํ๊ณ , ๋ฐ์ดํฐ๋ฒ ์ด์ค์ ์ํ๋ฅผ ์ผ๊ด๋๊ฒ ์ ์งํ๋ ๊ฒ์๋๋ค.

<br>

#### ๐กSQL๊ณผ NoSQL์ ์ฐจ์ด์ ์ ๋ํด ์ค๋ชํ์์ค

- SQL์ ๊ด๊ณํ ๋ฐ์ดํฐ๋ฒ ์ด์ค๋ก, ํ์ด๋ธ์ ๋ฐ์ดํฐ๋ฅผ ์ ์ฅํ๋ฉฐ ๋ค๋ฅธ ํ์ด๋ธ๊ณผ ๊ด๊ณ๋ฅผ ๋งบ๊ธฐ๋ ํฉ๋๋ค.

  ๋ฐ๋ฉด์, NoSQL์ ๊ตฌ์กฐ๋ฅผ ์ ์ํ์ง ์๊ณ  ๋ฐ์ดํฐ๋ฅผ ์ ์ฅํ๋ ๋ฐ์ดํฐ๋ฒ ์ด์ค์๋๋ค. NoSQL์ ๋ฌธ์, ํค-๊ฐ ๋ฑ์ ํํ๋ก ๋ฐ์ดํฐ๋ฅผ ์ ์ฅํฉ๋๋ค.

<br><br>

## ๐๐ปโโ๏ธ ์ ๋ฆฌ

### ๊ด๊ณํ ๋ฐ์ดํฐ๋ฒ ์ด์ค

- ํ์ด๋ธ๋ก ์ด๋ฃจ์ด์ ธ ์์ผ๋ฉฐ, ์ด ํ์ด๋ธ์ ํค(key)์ ๊ฐ(value)์ ๊ด๊ณ๋ฅผ ๋ํ๋ธ๋ค.
- ๋ฐ์ดํฐ์ ์ข์์ฑ์ ๊ด๊ณ(relationship)๋ก ํํํ๋ ๊ฒ์ด ๊ด๊ณํ ๋ฐ์ดํฐ๋ฒ ์ด์ค์ ํน์ง์ด๋ค.

![RDBMS](./src/RDBMS.png)

<br>

#### ํน์ง

- ๋ฐ์ดํฐ์ ๋ถ๋ฅ, ์ ๋ ฌ, ํ์ ์๋๊ฐ ๋น ๋ฅด๋ค.
- JOIN์ ํตํด์ ๋ฐ์ดํฐ๋ฅผ ์ป์ ์ ์์ผ๋ฏ๋ก ๋ฐ์ดํฐ ์ค๋ณต์ด ์ต์ํ๋๋๋ฐ, **๋ฐ์ดํฐ๋ฅผ ์ค๋ณตํด์ ์ ์ฅํ์ง ์๋๋ก ์ค๊ณํ๋ ๊ฒ์ด ๊ด๊ณํ ๋ฐ์ดํฐ๋ฒ ์ด์ค ์ค๊ณ์ ํต์ฌ**
- ๋ฐ์ดํฐ์ ๋ฌด๊ฒฐ์ฑ์ ๋ณด์ฅํ๋ค.
- ๊ธฐ์กด์ ์์ฑ๋ ์คํค๋ง๋ฅผ ์์ ํ๊ธฐ ์ด๋ ต๋ค.
- ๋ฐ์ดํฐ๋ฒ ์ด์ค์ ๋ถํ๋ฅผ ๋ถ์ํ๋ ๊ฒ์ด ์ด๋ ต๋ค.

<br>

<br>

### ๋ฌด๊ฒฐ์ฑ ์ ์ฝ์กฐ๊ฑด

- ๋ฐ์ดํฐ๋ฒ ์ด์ค์ ์ ์ฅ๋ ๋ฐ์ดํฐ์ ๋ฌด๊ฒฐ์ฑ์ ๋ณด์ฅํ๊ณ , ๋ฐ์ดํฐ๋ฒ ์ด์ค์ ์ํ๋ฅผ ์ผ๊ด๋๊ฒ ์ ์งํ๋ ๊ฒ

- **๋ฌด๊ฒฐ์ฑ?**

  ๋ฐ์ดํฐ์ ๊ฒฐํจ์ด ์๋ ์ํ. ์ฆ, ๋ฐ์ดํฐ๋ฅผ ์ ํํ๊ณ  ์ ํจํ๊ฒ ์ ์งํ๋ ๊ฒ

<br>

#### ์ข๋ฅ์ ๊ฐ๋

1. **๊ฐ์ฒด ๋ฌด๊ฒฐ์ฑ** : ๊ธฐ๋ณธํค๋ null ๊ฐ์ด ๋  ์ ์๋ค.

   - ๊ธฐ๋ณธํค๋ฅผ ๊ตฌ์ฑํ๋ ๋ชจ๋  ์์ฑ์ null ๊ฐ์ ๊ฐ์ง ์ ์๋ค๋ ๊ท์น

2. **์ฐธ์กฐ ๋ฌด๊ฒฐ์ฑ** : ์ธ๋ํค๋ ์ฐธ์กฐํ  ์ ์๋ ๊ฐ์ ๊ฐ์ง ์ ์๋ค.

   - ์ธ๋ํค : ๋ค๋ฅธ ๋ฆด๋ ์ด์์ ๊ธฐ๋ณธํค๋ฅผ ์ฐธ์กฐํ๋ ์์ฑ, ๋ฆด๋ ์ด์ ๊ฐ์ ๊ด๊ณ๋ฅผ ํํํ๋ ์ญํ 

   - ์ธ๋ํค๊ฐ ์์ ์ด ์ฐธ์กฐํ๋ ๋ฆด๋ ์ด์์ ๊ธฐ๋ณธํค์ ์๊ด์๋ ๊ฐ์ ๊ฐ์ง๊ฒ ๋๋ฉด ๋ ๋ฆด๋ ์ด์์ ์ฐ๊ด์ํฌ ์ ์์ผ๋ฏ๋ก ์ธ๋ํค ๋ณธ๋์ ์๋ฏธ๊ฐ ์์ด์ง๋ค.

3. **๋๋ฉ์ธ ๋ฌด๊ฒฐ์ฑ** : ํน์  ์์ฑ๊ฐ์ ๊ทธ ์์ฑ์ด ์ ์๋ ๋๋ฉ์ธ์ ์ํ ๊ฐ์ด์ด์ผ ํ๋ค.

   - ๊ฐ๊ฐ์ ์์ฑ์ ์ซ์, ๋ฌธ์ ๋ฑ์ ๋๋ฉ์ธ์ ๊ฐ์ง๋ฉด ํด๋น ๋๋ฉ์ธ์ ๋ง๋ ๋ฐ์ดํฐ๋ฅผ ์ฝ์ํด์ผ ํ๋ค.

4. **ํค ๋ฌด๊ฒฐ์ฑ** : ๋ฆด๋ ์ด์์๋ ์ต์ํ ํ๋์ ํค๊ฐ ์กด์ฌํด์ผ ํ๋ค.

5. **null ๋ฌด๊ฒฐ์ฑ** : ํน์  ์์ฑ์ null ๊ฐ์ ๊ฐ์ง ์ ์๋ค.

6. **๊ณ ์  ๋ฌด๊ฒฐ์ฑ** : ํน์  ์์ฑ๊ฐ์ ์๋ก ๋ฌ๋ผ์ผ ํ๋ค.

   - ํน์  ์์ฑ์ ์ฝ์๋๋ ๋ฐ์ดํฐ๋ ๊ณ ์ ํ ๊ฐ์ ๊ฐ์ ธ์ผ ํ๋ค๋ ๊ท์น์ด๋ค.
   - ์ฆ, ๊ฐ ํํ์์ ํ๋์ ์์ฑ๊ฐ์ ์ค๋ณต๋ ๊ฐ์ด ์๋ ๊ฐ๊ฐ ์๋ก ๋ค๋ฅธ ๊ฐ์ ๊ฐ์ ธ์ผ ํ๋ค๋ ์๋ฏธ

<br>

<br>

### NoSQL

- ๊ด๊ณํ ๋ฐ์ดํฐ๋ฒ ์ด์ค๊ฐ ์๋, ์ฌ๋ฌ ์ ํ์ ๋ฐ์ดํฐ๋ฒ ์ด์ค๋ฅผ ์ฌ์ฉํ๋ค.
- ๋ฐ์ดํฐ๋ฅผ ์กฐ์ํ๋ ๋ฐฉ๋ฒ์๋ ๋ฆฌ์คํธ, ํด์ ํ์ด๋ธ, ํธ๋ฆฌ, ๊ทธ๋ํ ๋ฑ ๋ค์ํ ๋ฐฉ๋ฒ์ด ์๋ค.

<br>

#### ํน์ง

- ๊ณ ์ ๋ ์คํค๋ง ๋ฐ JOIN์ด ์กด์ฌํ์ง ์๋๋ค. (์ ํด์ง ๊ท๊ฒฉ ์์)
- ์ํ์  ํ์ฅ ๊ธฐ๋ฅ์ ์ฝ๊ฒ ์ ๊ณตํ๋ค.

<br>

#### RDBMS์ NoSQL ๋น๊ต

|    ํน์ง     | RDBMS  | NoSQL  |
| :---------: | :----: | :----: |
| ์ ํด์ง ๊ท๊ฒฉ |   O    |   X    |
|    JOIN     |  ๊ฐ๋ฅ  | ๋ถ๊ฐ๋ฅ |
|  ํธ๋์ญ์   |  ์ฌ์ฉ  |  ์์  |
|  ๋ถ์ฐ์ฒ๋ฆฌ   | ์ด๋ ค์ |  ์ฌ์  |

##### RDBMS (SQL) ์ฌ์ฉ์ด ๋ ์ข์ ๊ฒฝ์ฐ

- ๊ด๊ณ๋ฅผ ๋งบ๊ณ  ์๋ ๋ฐ์ดํฐ๊ฐ ์์ฃผ ๋ณ๊ฒฝ๋๋ ๊ฒฝ์ฐ
- ๋ณ๊ฒฝ๋  ์ฌ์ง๊ฐ ์๊ณ , ๋ชํํ ์คํค๋ง๊ฐ ์ฌ์ฉ์์ ๋ฐ์ดํฐ์๊ฒ ์ค์ํ ๊ฒฝ์ฐ
- ex) ์ผํ๋ชฐ (์ ํ์ฑ์ด ์ค์ํ ๊ฒฝ์ฐ)

##### NoSQL ์ฌ์ฉ์ด ๋ ์ข์ ๊ฒฝ์ฐ

- ์ ํํ ๋ฐ์ดํฐ ๊ตฌ์กฐ๋ฅผ ์ ์ ์๊ฑฐ๋ ๋ณ๊ฒฝ/ํ์ฅ ๋  ์ ์๋ ๊ฒฝ์ฐ
- ์ฝ๊ธฐ๋ฅผ ์์ฃผ ํ์ง๋ง, ๋ฐ์ดํฐ ๋ณ๊ฒฝ์ ์์ฃผ ์๋ ๊ฒฝ์ฐ
- ๋ฐ์ดํฐ๋ฒ ์ด์ค๋ฅผ ์ํ์ ์ผ๋ก ํ์ฅํด์ผ ํ๋ ๊ฒฝ์ฐ (๋ง๋ํ ์์ ๋ฐ์ดํฐ๋ฅผ ๋ค๋ฃจ๋ ๊ฒฝ์ฐ)
- ex) ์ฑํ ๋ก๊ทธ ๊ฐ์ ๊ฒฝ์ฐ

<br>

---

**[์ฐธ๊ณ ]**

[๊ด๊ณํ ๋ฐ์ดํฐ๋ฒ ์ด์ค](http://tcpschool.com/mysql/mysql_intro_relationalDB)

[๊ด๊ณํ ๋ฐ์ดํฐ๋ฒ ์ด์ค 2](https://noahlogs.tistory.com/37)

[๊ด๊ณํ ๋ฐ์ดํฐ๋ฒ ์ด์ค 3](https://velog.io/@full_accel/%EA%B4%80%EA%B3%84%ED%98%95-%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4-%EA%B4%80%EA%B3%84%ED%98%95-%EB%AA%A8%EB%8D%B8%EC%9D%98-%EA%B8%B0%EB%B3%B8-%EA%B0%9C%EB%85%90%EA%B3%BC-%EC%9A%A9%EC%96%B4-%EC%A0%95%EC%9D%98)

[๋ฌด๊ฒฐ์ฑ ์ ์ฝ์กฐ๊ฑด](https://kosaf04pyh.tistory.com/202)

[SQL๊ณผ NoSQL ๋น๊ต](https://devuna.tistory.com/25)

[SQL๊ณผ NoSQL ๋น๊ต 2](https://mjmjmj98.tistory.com/43)

[SQL๊ณผ NoSQL ๋น๊ต 3](https://www.stevenjlee.net/2020/07/06/%EC%9D%B4%ED%95%B4%ED%95%98%EA%B8%B0-nosql-vs-sql-%EA%B7%B8%EB%A6%AC%EA%B3%A0-nosql-%EC%9D%98-%EC%A2%85%EB%A5%98/)

[SQL๊ณผ NoSQL ๋น๊ต 4](https://www.fun-coding.org/mongodb_basic1.html)

