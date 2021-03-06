## JAVA

#### ๐ก JVM ๊ตฌ์กฐ๋?

- JVM์ JAVA ๊ฐ์ ๋จธ์ ์ผ๋ก, JAVA ๋ฐ์ดํธ ์ฝ๋๋ฅผ ์คํํ  ์ ์๋ ์ฃผ์ฒด์ด๋ฉฐ,

  ํฌ๊ฒ (1) Class Loader, (2) GC(Garbage Collector), (3) Execute Engine, (4) Runtime Data Area ๋ค ๊ฐ์ง๋ก ๋๋ฉ๋๋ค.

  ๋จผ์ , ์๋ฐ ์ปดํ์ผ๋ฌ๊ฐ .java ํ์ผ์ ์ปดํ์ผํ๋ฉด ๋ฐ์ดํธ์ฝ๋๋ก ์ด๋ฃจ์ด์ง .class ํ์ผ์ด ์์ฑ๋ฉ๋๋ค.

  <b>Class Loader</b>๋ ์ด๋ ๊ฒ ์์ฑ๋ <u>ํด๋์ค ํ์ผ๋ค์ ์ฎ์ด</u> Runtime Data Area ํํ๋ก <u>๋ฉ๋ชจ๋ฆฌ์ ์ ์ฌ</u>ํ๋ ์ญํ ์ ํฉ๋๋ค.

  <b>Execution Engine</b>์ <u>๋ฉ๋ชจ๋ฆฌ์ ์ ์ฌ๋ ํด๋์ค๋ค์ ๊ธฐ๊ณ์ด๋ก ๋ณ๊ฒฝ</u>ํด <u>๋ช๋ น์ด ๋จ์๋ก ์คํ</u>ํ๋ ์ญํ ์ ํฉ๋๋ค.

  <b>Garbage Collector</b>๋ <u>Heap ๋ฉ๋ชจ๋ฆฌ ์์ญ</u>์ ์์ฑ๋ ๊ฐ์ฒด๋ค ์ค, <u>์ฐธ์กฐ๋์ง ์์ ๊ฐ์ฒด๋ฅผ ํ์ํ๊ณ  ์ ๊ฑฐ</u>ํ๋ ์ญํ ์ ํฉ๋๋ค.

  <b>Runtime Data Area</b>๋ <u>JVM์ ๋ฉ๋ชจ๋ฆฌ ์์ญ</u>์ผ๋ก ์๋ฐ ์ดํ๋ฆฌ์ผ์ด์ ์คํ์ ์ฌ์ฉ๋๋ ๋ฐ์ดํฐ๋ฅผ ์ ์ฌํ๋ ์์ญ์๋๋ค.

  ![img](./src/JVM.png)

<br>

#### ๐ก Java์ GC ์ฝ๋ ํฐ์ ์๋ ๋ฐฉ์์ ๋ฌด์์ธ๊ฐ์?

- <b>'stop-the-world'</b>๊ฐ ๋ฐ์ํ๋ฉด GC๋ฅผ ์คํํ๋ ์ฐ๋ ๋๋ฅผ ์ ์ธํ ๋๋จธ์ง ์ฐ๋ ๋๋ ๋ชจ๋ ์์์ ๋ฉ์ถฅ๋๋ค.

  stop-the-world๋ <u>GC๋ฅผ ์คํํ๊ธฐ ์ํด JVM์ด ์ดํ๋ฆฌ์ผ์ด์ ์คํ์ ๋ฉ์ถ๋ ๊ฒ</u>์ด๊ณ , ์์๋ค์ GC ์์์ ์๋ฃํ ์ดํ์์ผ ์ค๋จํ๋ ์์์ ๋ค์ ์์ํฉ๋๋ค.

- GC์ ๊ณผ์ ์ <b>Mark and Sweep</b>๋ผ๊ณ ๋ ํ๋๋ฐ, <u>GC๊ฐ ์คํ์ ๋ชจ๋  ๋ณ์ ๋๋ Reachable ๊ฐ์ฒด๋ฅผ ์ค์บํ๋ฉด์ ๊ฐ๊ฐ ์ด๋ค ๊ฐ์ฒด๋ฅผ ์ฐธ์กฐํ๊ณ  ์๋์ง ์ฐพ๋ ๊ณผ์ </u>์ด <b>Mark</b>์๋๋ค. ์ด ๊ณผ์ ์์ <u>stop-the-world</u>๊ฐ ๋ฐ์ํฉ๋๋ค.

  ์ดํ <u>Mark ๋์ด์์ง ์์ ๊ฐ์ฒด๋ค์ ํ์์ ์ ๊ฑฐํ๋ ๊ณผ์ </u>์ด <b>Sweep</b>์๋๋ค.

- GC๋ ๊ฐ๋น์ง ๊ฐ์ฒด๋ฅผ ํ๋ณํ๊ธฐ ์ํด reachability๋ผ๋ ๊ฐ๋์ ์ฌ์ฉํฉ๋๋ค.

  ์ด๋ค ๊ฐ์ฒด์ ์ ํจํ ์ฐธ์กฐ๊ฐ ์์ผ๋ฉด 'reachable', ์์ผ๋ฉด 'unreachable'๋ก ๊ตฌ๋ณํ๊ณ , 'unreachable' ๊ฐ์ฒด๋ฅผ ๊ฐ๋น์ง๋ก ๊ฐ์ฃผํฉ๋๋ค.

<br>

#### ๐ก Java SE์ EE์ ์ฐจ์ด์ ์ ๋ฌด์์ธ๊ฐ์?

- Java SE๋ ํ์ค ์๋์์ ์๋ฐ ํ๋ซํผ์ผ๋ก, ๊ฐ์ฅ ๋์ค์ ์ธ ์๋ฐ ํ๋ซํผ์๋๋ค. ํํ ์๋ฐ์ธ์ด๋ผ๊ณ  ํ๋ ๋๋ถ๋ถ์ ํจํค์ง๊ฐ ํฌํจ๋ ์๋์์๋๋ค.

  Java SE์ API๋ ์๋ฐ ํ๋ก๊ทธ๋๋ฐ ์ธ์ด์ ํต์ฌ ๊ธฐ๋ฅ๋ค์ ์ ๊ณตํฉ๋๋ค. (๊ธฐ์ด์ ์ธ ํ์, ๋คํธ์ํน, ๋ณด์, ๋ฐ์ดํฐ๋ฒ ์ด์ค ์ฒ๋ฆฌ, ๊ทธ๋ํฝ ์ฌ์ฉ์ ์ธํฐํ์ด์ค ๊ฐ๋ฐ, XML ํ์ฑ ๋ฑ..)

- Java EE๋ ์ํฐํ๋ผ์ด์ฆ ์๋์์ ์๋ฐ ํ๋ซํผ์ผ๋ก, Java SE ํ๋ซํผ์ ๊ธฐ๋ฐ์ผ๋ก ๊ทธ ์์ ํ์ฌ๋ฉ๋๋ค.

  ์น ํ๋ก๊ทธ๋๋ฐ์ ํ์ํ ๊ธฐ๋ฅ์ ๋ค์ ํฌํจํฉ๋๋ค. (JSP, Servlet, JDBC ๋ฑ..)

<br>

#### ๐ก ์ฐธ์กฐํ ๋ณ์์ ๊ธฐ๋ณธํ ๋ณ์์ ์ฐจ์ด์ ์ ์ค๋ชํด์ฃผ์ธ์.

- <b>๊ธฐ๋ณธํ ๋ณ์</b>๋ boolean, char, byte, short ๋ฑ๊ณผ ๊ฐ์ ํ์์ผ๋ก, <u>์ ์ฅ ๊ณต๊ฐ์ ๊ฐ ์์ฒด๋ฅผ ์ ์ฅ</u>ํฉ๋๋ค.

- <b>์ฐธ์กฐํ ๋ณ์</b>๋ ๊ธฐ๋ณธํ์ ์ ์ธํ ๋๋จธ์ง ํ์์ผ๋ก, String, StringBuffer, List ๋ฑ์ด๋ ๊ฐ์ธ์ด ๋ง๋  ํด๋์ค๋ ์ฐธ์กฐํ ํ์์ด ๊ฐ๋ฅํฉ๋๋ค. ์ฐธ์กฐํ ๋ณ์๋ <u>์ฐธ์กฐ ๊ฐ(์ฃผ์)๋ฅผ ๊ฐ๋ ์๋ฃํ</u>์ผ๋ก, ์๋ฐ API์์ ์ ๊ณต๋๊ฑฐ๋ ํ๋ก๊ทธ๋๋จธ์ ์ํด์ ๋ง๋ค์ด์ง ํด๋์ค๋ฅผ ์๋ฃํ์ผ๋ก ์ ์ธํ๋ ๊ฒฝ์ฐ์๋๋ค.

- ์ฆ, <b>๊ธฐ๋ณธํ ๋ณ์</b>๋ ๋ฆฌํฐ๋ด (์ค์  ๊ฐ)์ด ์ ์ฅํ๋ ๊ณต๊ฐ์ผ๋ก <u>์คํ(Stack) ๋ฉ๋ชจ๋ฆฌ</u>์ ์ ์ฅ๋๋ค๋ฉด,

  <b>์ฐธ์กฐํ ๋ณ์</b>๋ ๊ฐ์ด ์ ์ฅ๋์ด ์๋ ๊ณณ์ ์ฃผ์ ๊ฐ์ ์ ์ฅํ๋ ๊ณต๊ฐ์ผ๋ก <u>ํ(Heap) ๋ฉ๋ชจ๋ฆฌ</u>์ ์ ์ฅ๋ฉ๋๋ค.

<br>

#### ๐ก public ์ ๊ทผ ์ ์ด์์ private ์ ๊ทผ ์ ์ด์์ ์ฐจ์ด

- <b>public ์ ๊ทผ ์ ์ด์</b>๋ฅผ ์ฌ์ฉํ์ฌ ์ ์ธ๋ ํด๋์ค ๋ฉค๋ฒ๋ ์ธ๋ถ๋ก ๊ณต๊ฐ๋๋ฉฐ, <u>ํด๋น ๊ฐ์ฒด๋ฅผ ์ฌ์ฉํ๋ ํ๋ก๊ทธ๋จ ์ด๋์์๋ ์ง์  ์ ๊ทผํ  ์ ์์ต๋๋ค.</u>

  ![img](./src/public.png)

- <b>private ์ ๊ทผ ์ ์ด์</b>๋ฅผ ์ฌ์ฉํ์ฌ ์ ์ธ๋ ํด๋์ค ๋ฉค๋ฒ๋ ์ธ๋ถ์ ๊ณต๊ฐ๋์ง ์์ผ๋ฉฐ, <u>์ธ๋ถ์์๋ ์ง์  ์ ๊ทผํ  ์ ์์ต๋๋ค.</u>

  ์ฆ, ์๋ฐ ํ๋ก๊ทธ๋จ์ private ๋ฉค๋ฒ์ ์ง์  ์ ๊ทผํ  ์ ์์ผ๋ฉฐ, <u>ํด๋น ๊ฐ์ฒด์ public ๋ฉ์๋๋ฅผ ํตํด์๋ง ์ ๊ทผํ  ์ ์์ต๋๋ค.</u>

  ![img](./src/private.png)

<br>

#### ๐ก non-static ๋ฉค๋ฒ์ static ๋ฉค๋ฒ์ ์ฐจ์ด์ ๋ํด ์ค๋ชํ์์ค.

- static ๋ฉค๋ฒ๋ ํ๋ก๊ทธ๋จ ์์์ ์ต์ด์ ๋จ ํ ๋ฒ๋ง ์์ฑ๋๊ณ  ์ด๊ธฐํ๋๋ฉฐ, ์ธ์คํด์ค๋ฅผ ์์ฑํ์ง ์๊ณ ๋ ๋ฐ๋ก ์ฌ์ฉํ  ์ ์์ต๋๋ค. ๋ํ, ํด๋น ํด๋์ค์ ๋ชจ๋  ์ธ์คํด์ค๊ฐ ๊ณต์ ํฉ๋๋ค.

- ์ฝ๋๋ฅผ ์คํํ๋ฉด ๋จผ์  static ๋ฉค๋ฒ๋ค์ด ๋ฉ์๋ ์์ญ์ ์ ์ฅ๋๊ฒ ๋ฉ๋๋ค. static ๋ฉ์๋์ ๋ฉค๋ฒ ๋ณ์์ ๊ด๋ จ ์ ๋ณด๋ค์ ์คํ(Stack) ์์ญ์ ์ ์ฅ๋ฉ๋๋ค. ํ์ง๋ง, non-static ๋ฉค๋ฒ๋ ๋ฉ๋ชจ๋ฆฌ์ ์ฌ๋ผ๊ฐ์ง ์์ต๋๋ค.

- <b>static ๋ฉค</b>/๋ ํด๋์ค ๋ด์ static ํค์๋๋ก ์ ์ธ๋ ๋ณ์๋ก, ์ฒ์ <u>JVM์ด ์คํ๋์ด ํด๋์ค๊ฐ ๋ฉ๋ชจ๋ฆฌ์ ์ฌ๋ผ๊ฐ ๋๋ถํฐ ํ๋ก๊ทธ๋จ์ด ์ข๋ฃ๋  ๋๊น์ง ์ ์ง</u>๋ฉ๋๋ค.

  ํด๋์ค๊ฐ ์ฌ๋ฌ๋ฒ ์์ฑ๋์ด๋ static ๋ณ์๋ <u>์ฒ์ ๋ฑ ํ ๋ฒ๋ง ์์ฑ</u>๋๊ณ , <u>๋์ผํ ํด๋์ค์ ๋ชจ๋  ๊ฐ์ฒด๋ค์ ์ํด์ ๊ณต์ </u>๋ฉ๋๋ค.

- <b>non-static ๋ฉค๋ฒ</b>๋ ํด๋์ค ๋ด์ ์ ์ธ๋ ๋ณ์๋ก, <u>๊ฐ์ฒด ์์ฑ ์๋ง๋ค ๋งค๋ฒ ์๋ก์ด ๋ณ์๊ฐ ์์ฑ</u>๋ฉ๋๋ค. ๋ํ, ํด๋์ค ๋ณ์์ ๋ฌ๋ฆฌ ๊ณต์ ๋์ง ์์ต๋๋ค.

<br>

#### ๐ก main ๋ฉ์๋๊ฐ public static์ธ ์ด์ ๋?

- ๋จผ์ , <b>public</b>์ ์ ๊ทผ ์ ์ด์๋ก, <u>JVM์ด ์ ๊ทผํ๊ธฐ ์ํด์ public์ ์ฌ์ฉ</u>ํด์ผ๋ง ํฉ๋๋ค. ๋ค๋ฅธ ์ ๊ทผ ์ ์ด์๋ฅผ ์ฌ์ฉํ๋ฉด ํ๋ก๊ทธ๋จ์ด ์คํ๋์ง ์์ต๋๋ค. (ํด๋์ค๊ฐ ์ด๋ ์์น์ ์๊ฑด JVM์ด ์ ๊ทผ ๊ฐ๋ฅํ๋๋ก ํ๊ธฐ ์ํด)
- main ๋ฉ์๋๋ <u>ํ๋ก๊ทธ๋จ์ด ์คํ๋๋ฉด ์ ์ผ ๋จผ์  ํธ์ถ๋๋ ๋ฉ์๋</u>์ด๊ธฐ ๋๋ฌธ์ <u>๊ฐ์ฒด๋ฅผ ์์ฑํ์ง ์์ ์ฑ๋ก ๋ฐ๋ก ์์์ ์ํํด์ผ ํ๊ธฐ ๋๋ฌธ์</u> <b>static</b> ์ด์ด์ผ ํฉ๋๋ค.

<br>

#### ๐ก Final ํค์๋์ ์ฉ๋์ ๋ํด ์ค๋ชํ์์ค.

- final์ '์ต์ข์ '์ด๋ผ๋ ์๋ฏธ๋ก ๋ฉค๋ฒ ๋ณ์์ ํด๋์ค, ๋ฉ์๋ ๊ทธ๋ฆฌ๊ณ  ๋ฉ์๋ ์ธ์์ ๋ถ์ผ ์ ์์ต๋๋ค.

  <b>final ๋ฉค๋ฒ ๋ณ์</b>๋ <u>๋ณ์์ ๊ฐ ํ ๋น์ ๋ฑ ํ ๋ฒ</u> ํ  ์ ์์ต๋๋ค. ๋ง์ฝ ๋ฉค๋ฒ ๋ณ์๋ฅผ final๋ก ์ ์ธํ๊ณ , ์ ์ธ๋ถ์ ์์ฑ์์์ ์ด๊ธฐํํ์ง ์์ผ๋ฉด ์ปดํ์ผ ์๋ฌ๊ฐ ๋ฐ์ํฉ๋๋ค. <u>๊ฐ์ฒด๊ฐ ์์ฑ๋๊ณ  ๋ ์ดํ์๋ ์์์ฒ๋ผ ์์ฉํด์ผ ํ๋ ํน์ฑ์ ๋ฉค๋ฒ ๋ณ์ ์์ ์ฌ์ฉ</u>ํฉ๋๋ค.

  ~~~java
  private final int number = 0;
  ~~~

  <b>final ๋ณ์</b>๋ final ๋ฉค๋ฒ ๋ณ์์ ๋ง์ฐฌ๊ฐ์ง๋ก ์ต์ด ํ ๋ฒ๋ง ํ ๋นํ  ์ ์๊ณ , ์ดํ ๋ค์ ํ ๋นํ  ์ ์์ต๋๋ค. ๋ณ์๊ฐ ๊ฐ์ฒด์ ๋ํ ์ฐธ์กฐ์ธ ๊ฒฝ์ฐ์๋ ์ต์ด ์ฐธ์กฐํ๋ ๊ฐ์ฒด ์ด์ธ์ ๋ค๋ฅธ ๊ฐ์ฒด๋ฅผ ์ฐธ์กฐํ  ์ ์์ต๋๋ค. 

  ๋ณ์๊ฐ ๋ค๋ฅธ ๊ฐ์ฒด๋ฅผ ์ฐธ์กฐํ๋๋ก ๋ฐ๊ฟ ์๋ ์์ง๋ง, ์ฐธ์กฐ๋ ๊ฐ์ฒด์ ๋ฉ์๋๋ฅผ ํตํ ๊ฐ์ฒด ์์ฒด์ ๊ฐ์ ๋ฐ๊ฟ ์ ์์ต๋๋ค.

  ~~~java
  final Person person = new Person("Eric");
  person = new Person("Tom"); // Compile Error
  ~~~

  <b>final ํด๋์ค</b>๋ ๋ค๋ฅธ ํด๋์ค๊ฐ ์์ํ  ์ ์์ต๋๋ค. ํน์  ํด๋์ค๋ฅผ ์์ํ๋ฉด์ ๋ฉ์๋๋ค์ ์ค๋ฒ๋ผ์ด๋ํด์ ์ฌ์ฉํ๋ ๊ฒฝ์ฐ๋ฅผ ๋ง๊ณ  ์ถ์ ๊ฒฝ์ฐ, final ํค์๋๋ฅผ ํด๋์ค ์์ ๋ถ์ฌ์ฃผ๋ฉด ๋ฉ๋๋ค.

  ~~~java
  final class Person {
    String name;
  }
  
  // ์์ ๋ถ๊ฐ๋ฅ
  class Doctor extends Person {
    
  }
  ~~~

  <b>final ๋ฉ์๋</b>๋ฅผ ์ฌ์ฉํ๋ ๊ฒฝ์ฐ, ์ฆ ํด๋์ค ์ ์์ final ํค์๋๋ฅผ ๋ฉ์๋ ์์ ๋ถ์ด๋ฉด, <u>ํด๋น ๋ฉ์๋๋ฅผ ์ค๋ฒ๋ผ์ด๋ ํ  ์ ์์ต๋๋ค.</u> ํด๋์ค๋ฅผ ์ ์ํ๋ฉด์ ์์์ ํ์ฉํ๋, ์ฝ์ด ๋ก์ง์ ์ค๋ฒ๋ผ์ด๋ ํ  ์ ์๋๋ก ๋ง๋ค๊ณ  ์ถ๋ค๋ฉด ๋ฉ์๋์ fiinal ํค์๋๋ฅผ ๋ถ์ด๋ฉด ๋ฉ๋๋ค.

  ~~~java
  public class Person {
    String name = "";
    public final void setName(String name) {
      this.name = name;
    }
  }
  
  public class Doctor extends Person {
    // ์ค๋ฒ๋ผ์ด๋ ๋ถ๊ฐ๋ฅ
    public void setName(String name) {
      this.name = "Doctor " + name;
    }
  }
  ~~~

  

<br>

#### ๐ก Generic์ ๋ํด ์ค๋ชํ์์ค.

- <b>Generic(์ ๋ค๋ฆญ)</b>์ด๋ <u>๋ฐ์ดํฐ์ ํ์์ ์ผ๋ฐํํ๋ค</u>๋ ๊ฒ์ ์๋ฏธํฉ๋๋ค. ์ ๋ค๋ฆญ์ <u>ํด๋์ค๋ ๋ฉ์๋์์ ์ฌ์ฉํ  ๋ด๋ถ ๋ฐ์ดํฐ ํ์์ ์ปดํ์ผ ์์ ๋ฏธ๋ฆฌ ์ง์ ํ๋ ๋ฐฉ๋ฒ</u>์๋๋ค.

  ์ด๋ ๊ฒ ์ปดํ์ผ ์์ ๋ฏธ๋ฆฌ ํ์ ๊ฒ์ฌ(type check)๋ฅผ ์ํํ๋ฉด ๋ค์๊ณผ ๊ฐ์ ์ฅ์ ์ ๊ฐ์ง๋๋ค.

  1. ํด๋์ค๋ ๋ฉ์๋ ๋ด๋ถ์์ ์ฌ์ฉ๋๋ ๊ฐ์ฒด์ ํ์ ์์ ์ฑ์ ๋์ผ ์ ์์ต๋๋ค.
  2. ๋ฐํ๊ฐ์ ๋ํ ํ์ ๋ณํ ๋ฐ ํ์ ๊ฒ์ฌ์ ๋ค์ด๊ฐ๋ ๋ธ๋ ฅ์ ์ค์ผ ์ ์์ต๋๋ค.

  ~~~java
  class MyArray<T> {
    T element;
    void setElement(T element) { this.element = element }
    T getElement() { return element; }
  }
  ~~~

  

<br>

#### ๐ก ==๊ณผ equals()์ ์ฐจ์ด์ ๋ํด ์ค๋ชํ์ธ์.

- equals()๋ ๋ฉ์๋๋ก, ๊ฐ์ฒด๋ผ๋ฆฌ ๋ด์ฉ์ ๋น๊ตํ  ์ ์๋ค. ์ฆ, ๋์์ ๋ด์ฉ ์์ฒด๋ฅผ ๋น๊ตํ๋ค.

- == ๋ ๋น๊ต๋ฅผ ์ํ ์ฐ์ฐ์๋ก, ๋น๊ตํ๊ณ ์ ํ๋ ๋์์ ์ฃผ์๊ฐ์ ๋น๊ตํ๋ค.

- <b>== ์ฐ์ฐ์</b>๋ <u>Call By Reference</u> (๋์์ ์ ์ธํ์ ๋, ์ฃผ์๊ฐ ๋ถ์ฌ)์ ๋ฐ๋ผ์ ํด๋น ๊ฐ์ฒด๋ ๋ณ์์ <u>์ฃผ์๊ฐ</u>์ ํตํ ๋น๊ต์ด๊ณ ,

  <b>equals() ๋ฉ์๋</b>๋ <u>Call By Value</u> (๊ธฐ๋ณธ์ ์ผ๋ก ๋์์ ์ฃผ์๊ฐ์ ๊ฐ์ง์ง ์๋ ๊ฒ์ผ๋ก ๊ฐ์ ํ ๋น๋ฐ๋ ํํ)์ ๋ฐ๋ผ ํด๋น ๋ณ์์ <u>value ๊ฐ ์์ฒด๋ฅผ ๋น๊ต</u>ํ์ฌ boolean ๊ฐ์ ๋ฐํํ๋ค.

~~~java
String a = "bbb";
String b = a;
String c = new String("bbb");

// Call By Reference
System.out.println(a == b); // true
System.out.println(a == c); // false
System.out.println(b == c); // false

// Call By Value
System.out.println(a.equals(b)); // true
System.out.println(a.equals(c)); // true
System.out.println(b.equals(c)); // true
~~~

<br>

#### ๐ก Call by Reference์ Call by Value์ ์ฐจ์ด์ ๋ํด ์ค๋ชํ์์ค.

- <b>Call By Value</b> (๊ฐ์ ์ํ ํธ์ถ)์ ํจ์์ ์ธ์๋ฅผ ์ ๋ฌํ  ๋ <u>'๊ฐ์ ์ ๋ฌํ๋ ๋ฐฉ์'</u>์ด๊ณ ,

  <b>Call By Reference</b> (์ฃผ์์ ์ํ ํธ์ถ)์ <u>'์ฃผ์๋ฅผ ์ ๋ฌํ๋ ๋ฐฉ์'</u>์๋๋ค.

  Java๋ Call By Value ๋ฐฉ์์ ์ฌ์ฉํฉ๋๋ค.

- Call By Value๋ '๊ฐ๋ง ์ ๋ฌํ๋ ๋ฐฉ์'์๋๋ค. ๋ง์ฝ ํจ์ A์์ B๋ก int ๋ณ์๋ฅผ ์ ๋ฌํ๋ค๊ณ  ํ์ ๋, ๋๊ฒจ๋ฐ์ B์์ ์ด๋ค ํ๋์ ํ๋์ง ๋ณ์์๋ ๋ณํจ์ด ์์ต๋๋ค.

  ![](./src/call-by-value.png)

  ![](./src/call-by-value-result.png)

- ![](./src/call-by-value-object.png)

  ![](./src/call-by-value-object-result.png)

  ์์ ๊ฐ์ ๊ฒฐ๊ณผ๊ฐ ๋์ค๋ ์ด์ ๋, ์ฐธ์กฐํ ๋ณ์๋ ์ฃผ์๋ฅผ ๊ฐ๊ณ  ์๊ธฐ ๋๋ฌธ์, Heap Memeory์ ์ฃผ์๊ฐ์ ๋๊ฒจ์ค๋ค! ํด๋น ์ฃผ์๊ฐ์ age์ name์ ๋ฐ๊พธ๋ ๊ฒ์ด๋ฏ๋ก ๋ฐ๋ ๊ฒฐ๊ณผ๊ฐ ๋์ค๋ ๊ฒ์ด๋ค.

<br>

#### ๐ก ์ถ์ ํด๋์ค์ ์ธํฐํ์ด์ค์ ์ฐจ์ด์ ๋ํด ์ค๋ชํ์์ค.

- <b>์ถ์ ํด๋์ค</b>๋ <u>ํ ๊ฐ ์ด์์ ์ถ์ ๋ฉ์๋๋ฅผ ๊ฐ๋ ํด๋์ค</u>๋ก, ์ถ์ ๋ฉ์๋๋ ๋ด์ฉ์ด ์๋ ๋ฉ์๋์ด๋ค. ์ฆ, ๊ตฌํ์ ํ์ง ์๊ณ  ์ ์ธ๋ง ํ ๋ฉ์๋์ด๋ค.

  ~~~java
  public abstract class AbstractTest {
    // ์ถ์ ๋ฉ์๋
    public abstract void dogName(String name);
    
    // ์ผ๋ฐ ๋ฉ์๋
    public void dog() {
  		System.out.println("์์");
    }
  }
  ~~~

  

- <b>์ธํฐํ์ด์ค</b>๋ <u>์ถ์๋ฉ์๋์ ์์๋ก๋ง ์ด๋ฃจ์ด์ ธ ์๋ ๊ฒ</u>์ผ๋ก, ๋ก์ง์ ์์ฑํ  ์ ์๋ค.

  ์ธํฐํ์ด์ค๋ <u>๋ค์ค ์์์ด ๊ฐ๋ฅ</u>ํ๋ค.

  ~~~java
  // ์ธํฐํ์ด์ค ํ์
  public interface DogTest {
    void LargeDog();
    void SmallDog();
  }
  
  // ์ธํฐํ์ด์ค ๋ค์ค ์์ ๊ฐ๋ฅ
  public interface ์ธํฐํ์ด์ค๋ช extends ์์๋ฐ์ ์ธํฐํ์ด์ค๋ช1, ์์๋ฐ์ ์ธํฐํ์ด์ค๋ช2, ... {
    void ์ถ์๋ฉ์๋1();
    ...
  }
  ~~~

  

<br>

#### ๐ก Java reflection์ ๋ํด ์ค๋ชํ์์ค.

- <b>Java Reflection</b>์ด๋ <u>๊ตฌ์ฒด์ ์ธ ํด๋์ค ํ์์ ์์ง ๋ชปํด๋ ๊ทธ ํด๋์ค์ ๋ฉ์๋, ํ์, ๋ณ์๋ค์ ์ ๊ทผํ  ์ ์๋๋ก ํด์ฃผ๋ ์๋ฐ API</u>์๋๋ค.

  ์ฝ๋๋ฅผ ์์ฑํ  ์์ ์๋ ์ด๋ค ํ์์ ํด๋์ค๋ฅผ ์ฌ์ฉํ ์ง ๋ชจ๋ฅด์ง๋ง, ๋ฐํ์ ์์ ์ ์ง๊ธ ์คํ๋๊ณ  ์๋ ํด๋์ค๋ฅผ ๊ฐ์ ธ์์ ์คํํด์ผ ํ๋ ๊ฒฝ์ฐ์ ์ฌ์ฉ๋ฉ๋๋ค.

- ์ฆ, ์ด๋ฏธ ๋ก๋ฉ์ด ์๋ฃ๋ ํด๋์ค์์ ๋ ๋ค๋ฅธ ํด๋์ค๋ฅผ ๋์ ์ผ๋ก ๋ก๋ฉ(Dynamic Loading)ํ์ฌ ์์ฑ์, ๋ฉค๋ฒ ํ๋ ๊ทธ๋ฆฌ๊ณ  ๋ฉค๋ฒ ๋ฉ์๋ ๋ฑ์ ์ฌ์ฉํ  ์ ์๋๋ก ํฉ๋๋ค.

  ์ปดํ์ผ ์๊ฐ(Compile Time)์ด ์๋๋ผ ์คํ ์๊ฐ(Run Time)์ ๋์ ์ผ๋ก ํน์  ํด๋์ค์ ์ ๋ณด๋ฅผ ๊ฐ์ฒดํ๋ฅผ ํตํด ๋ถ์ ๋ฐ ์ถ์ถํด๋ผ ์ ์๋ ํ๋ก๊ทธ๋๋ฐ ๊ธฐ๋ฒ์ด๋ผ๊ณ  ํํํ  ์ ์์ต๋๋ค.

<br>

#### ๐ก String๊ณผ StringBuilder์ StringBuffer์ ์ฐจ์ด์ ์ ์ค๋ชํด์ฃผ์ธ์.

- <b>String</b>์ ๋ถ๋ณ์ผ๋ก, ํ ๋ฒ ์์ฑ๋๋ฉด ๋ฌธ์์ด์ด ํ ๋น๋ ๋ฉ๋ชจ๋ฆฌ ๊ณต๊ฐ์ด ๋ณํ์ง ์์ต๋๋ค. ์ฆ, <u>๋ฌธ์์ด์ + ์ฐ์ฐ์ ๋ฑ์ ์ด์ฉํด ๋ค๋ฅธ ๋ฌธ์์ด์ ์ถ๊ฐํ  ๋,</u> ๊ธฐ์กด ๋ฌธ์์ด์ ์๋ก์ด ๋ฌธ์์ด์ด ์ถ๊ฐ๋๋ ๊ฒ ์๋๋ผ <u>์๋ก์ด ๋ฌธ์์ด ๊ฐ์ฒด๋ฅผ ๋ง๋ค๊ณ  ๊ทธ ๊ฐ์ฒด๋ฅผ ์ฐธ์กฐ</u>ํ๊ฒ ํฉ๋๋ค.

- <b>StringBuilder</b>์ <b>StringBuffer</b>๋ ๋ชจ๋ ๋ฌธ์์ด์ ํ ๋ฒ ๋ง๋ค๊ณ , <u>์ฐ์ฐ์ด ํ์ํ  ๋๋ง๋ค ํฌ๊ธฐ๋ฅผ ๋ณ๊ฒฝํด๊ฐ๋ฉฐ ๋ฌธ์์ด์ ๋ณ๊ฒฝ</u>ํ๋ค๋ ๊ณตํต์ ์ด ์์ต๋๋ค. ๋ ๊ฐ์ง์ ๊ฐ์ฅ ํฐ ์ฐจ์ด์ ์ ๋๊ธฐํ์๋๋ค.

- <b>StringBuilder</b>๋ <u>๋๊ธฐํ๋ฅผ ๋ณด์ฅํ์ง ์์ง๋ง</u>, <b>StringBuffer</b>๋ <u>๋๊ธฐํ๋ฅผ ๋ณด์ฅ</u>ํฉ๋๋ค.

  ![](./src/String&StringBuffer&StringBuilder.png)

<br>

#### ๐ก Java 8์ ์ถ๊ฐ๋ ๊ธฐ๋ฅ์ ๋ฌด์์ด ์๋์?

- Lambda ํํ์, Optional, ์ธํฐํ์ด์ค์ default method, Stream ๋ฑ์ด ์์ต๋๋ค.

- <b>Lambda ํํ์</b>์ ์ต๋ช ํด๋์ค๋ฅผ ์ฌ์ฉํ  ๊ฒฝ์ฐ, ๊ฐ๋์ฑ์ด ๋จ์ด์ง๋ ๋ถํธํจ์ ๋ณด์ํฉ๋๋ค.

  ๋์ , ์ด ํํ์์ ์ธํฐํ์ด์ค์ ๋ฉ์๋๊ฐ ํ๋์ธ ๊ฒ๋ค๋ง ์ ์ฉ ๊ฐ๋ฅํฉ๋๋ค.

  ~~~java
  ๋งค๊ฐ๋ณ์ ๋ชฉ๋ก (int x, int y)
  ํ์ดํ ํ ํฐ(Arrow Token) ->
  ์ฒ๋ฆฌ ์ x + y (ํ ์ค ์ด์์ผ ๋์๋ ์ค๊ดํธ๋ก ๋ฌถ์ ์ ์๋ค)
  ์ข์ธก์๋ ๋๊ฒจ์ง๋ ๋งค๊ฐ ๋ณ์๋ค์ ํ์์ด ์ ์ธ๋๊ณ , ์ค๊ฐ์๋ ํ์ดํ ์ฐ์ฐ์, ๊ฐ์ฅ ์ฐ์ธก์๋ ๋ฆฌํด๋๋ ๊ฐ์ ํ์ํ๋ค.
  ~~~

- <b>Optional</b>์ <u>null ์ฒ๋ฆฌ๋ฅผ ๋ณด๋ค ๊ฐํธํ๊ฒ</u> ํ๊ธฐ ์ํด ๋ง๋ค์ด์ก์ต๋๋ค. ๋ฐ์ดํฐ๊ฐ ์์ ๊ฒฝ์ฐ, null์ ๋ฆฌํดํ๊ณ , ๊ฐ์ด ์์ ๊ฒฝ์ฐ์๋ ๊ธฐ๋ณธ๊ฐ์ ์ง์ ํ  ์ ์์ต๋๋ค.

- <b>์ธํฐํ์ด์ค์ default method</b>๋ <u>์ธํฐํ์ด์ค ์์ ๊ตฌํ๋ ๋ฉ์๋๋ฅผ ์ถ๊ฐํด์ผ ํ  ๋ default ํค์๋</u>๋ฅผ ๋ถ์ฌ ์ฌ์ฉํฉ๋๋ค.

  default method๋ฅผ ๋ง๋  ์ด์ ๋ <u>'ํ์ ํธํ์ฑ'</u> ๋๋ฌธ์๋๋ค. ๋ง์ ์ฌ๋์ด ์ฌ์ฉํ๊ณ  ์๋ ์ธํฐํ์ด์ค์ ์๋ก์ด ๋ฉ์๋๋ฅผ ์ถ๊ฐํด์ผ ํ  ๋, ๊ธฐ์กด ๋ฐฉ์๋๋ก ์ถ๊ฐํ๋ฉด ์ด๋ฏธ ์ฌ์ฉํ๊ณ  ์๋ ์ฌ๋๋ค์ ์ ๋ถ ์ค๋ฅ๊ฐ ๋ฐ์ํ๊ณ  ์์ ํด์ผ ํ๋ ์ผ์ด ๋ฐ์ํฉ๋๋ค. ์ด๋ด ๋ ์ฌ์ฉํ๋ ๊ฒ์ด default ๋ฉ์๋์๋๋ค.

- <b>Stream</b>์ ๋ญ๊ฐ <u>์ฐ์๋ ์ ๋ณด๋ฅผ ์ฒ๋ฆฌ</u>ํ๋ ๋ฐ ์ฌ์ฉํฉ๋๋ค. Stream()์ ์์ฐจ์ ์ผ๋ก ๋ฐ์ดํฐ๋ฅผ ์ฒ๋ฆฌํฉ๋๋ค. (index์)

<br>

#### ๐ก Lambda๋ ๋ฌด์์ด๊ณ  ์ด๋ ํ ์ฅ์ ์ด ์๋๊ฐ?

- <b>๋๋ค ํํ์</b>์ ๋ฉ์๋๋ก ์ ๋ฌํ  ์ ์๋ ์ต๋ช ํจ์(anonymous function)์ ์์ฑํ๊ธฐ ์ํ ์์๋๋ค.

  <u>๋งค๊ฐ ๋ณ์๋ฅผ ๊ฐ์ง ์ฝ๋ ๋ธ๋ญ์ด์ง๋ง, ๋ฐํ์์์๋ ์ต๋ช ๊ตฌํ ๊ฐ์ฒด๋ฅผ ์์ฑ</u>ํฉ๋๋ค.

  ์ต๋ช ํด๋์ค๋ ์์ฑํ  ๋ ๋ง์ ์ฝ๋๋ฅผ ์์ฑํด์ผ ํ์ง๋ง, ๋๋ค๋ ๋ถํ์ํ ์ฝ๋๋ฅผ ์์ฑํ์ง ์์๋ ๋๋ค๋ ์ฅ์ ์ด ์์ต๋๋ค.

  ~~~java
  // ์ธํฐํ์ด์ค์ ์ต๋ช ๊ตฌํ ๊ฐ์ฒด
  Runnable runnable = new Runnable() {
    public void run() { ... }
  }
  
  // ๋๋ค์
  Runnable runnable = () -> { ... };
  ์ธํฐํ์ด์ค ๋ณ์๋ช = ๋๋ค์;
  ~~~

<br>

#### ๐ก ์์ธ์ฒ๋ฆฌ ๋ฐฉ๋ฒ์ ์ค๋ชํด์ฃผ์ธ์.

- ์์ธ ์ฒ๋ฆฌ ๋ฐฉ๋ฒ์๋ ์ธ ๊ฐ์ง๊ฐ ์์ต๋๋ค.

- <b>์์ ๋ณต๊ตฌ</b>๋ <u>์์ธ ์ํฉ์ ํ์ํ๊ณ , ๋ฌธ์ ๋ฅผ ํด๊ฒฐํด์ ์ ์ ์ํ๋ก ๋๋ ค๋๋ ๊ฒ</u>์๋๋ค.

  ๋ง์ฝ ์์ธ๋ก ์ด๋ค ์์์ ์ฒ๋ฆฌ๊ฐ ๋ถ๊ฐ๋ฅํ๋ค๋ฉด ๋ค๋ฅด๊ฒ ์์์ ์ฒ๋ฆฌํ๋๋ก ์ ๋ํจ์ผ๋ก์จ ์์ธ๋ฅผ ์ฒ๋ฆฌํ๋ ๋ฐฉ๋ฒ์๋๋ค.

- <b>์์ธ ์ฒ๋ฆฌ ํํผ</b>๋ <u>์์ธ ์ฒ๋ฆฌ๋ฅผ ์ง์  ์ฒ๋ฆฌํ์ง ์๊ณ , ์์ ์ ํธ์ถํ ๊ณณ์ผ๋ก ๋์ ธ๋ฒ๋ฆฌ๋ ๊ฒ</u>์๋๋ค.

  ๋ง์ฝ ํด๋น ์์ธ๋ฅผ ์ฒ๋ฆฌํ๋ ๊ฒ์ด ์์ ์ด ํด์ผ๋  ์ผ์ด ์๋๋ผ๊ณ  ๋๊ปด์ง๋ค๋ฉด ๋ค๋ฅธ ๋ฉ์๋์์ ์ฒ๋ฆฌํ๋๋ก ๋๊ฒจ์ค ๋ ์ฌ์ฉํฉ๋๋ค. ํ์ง๋ง ๋ฌด์์  ์์ธ๋ฅผ ๋๊ฒจ์ฃผ๋ ๊ฒ์ ๋ฌด์ฑ์ํ ํํผ๊ฐ ๋  ์ ์์ผ๋ฏ๋ก ์ํฉ์ ๋ฐ๋ผ ์ ์ ํ๊ฒ ์ฌ์ฉํด์ผ ํฉ๋๋ค.

- <b>์์ธ ์ ํ</b>์ ์์ธ ํํผ์ ๋ง์ฐฌ๊ฐ์ง๋ก <u>์์ธ๋ฅผ ๋ณต๊ตฌํ  ์ ์๋ ์ํฉ์ ์ฌ์ฉ</u>๋๋ฉฐ, ์์ธ์ฒ๋ฆฌ ํํผ์ ๋ค๋ฅด๊ฒ <u>์ ์ ํ ์์ธ๋ก ๋ณํํ์ฌ ๋์ง๋ค๋ ํน์ง</u>์ด ์์ต๋๋ค.

<br>

#### ๐ก Collection ์ ์์ ์ข๋ฅ๋ฅผ ๋ง์ํด์ฃผ์ธ์

- ์๋ฐ์์ <b>์ปฌ๋ ์ ํ๋ ์์ํฌ</b>๋, ๋ค์์ ๋ฐ์ดํฐ๋ฅผ ์ฝ๊ณ  ํจ๊ณผ์ ์ผ๋ก ์ฒ๋ฆฌํ  ์ ์๋ ํ์คํ๋ ๋ฐฉ๋ฒ์ ์ ๊ณตํ๋ ํด๋์ค์ ์งํฉ์ ์๋ฏธํฉ๋๋ค.

  ์ฆ, <u>๋ฐ์ดํฐ๋ฅผ ์ ์ฅํ๋ ์๋ฃ๊ตฌ์กฐ์ ๋ฐ์ดํฐ๋ฅผ ์ฒ๋ฆฌํ๋ ์๊ณ ๋ฆฌ์ฆ์ ๊ตฌ์กฐํํ์ฌ ํด๋์ค๋ก ๊ตฌํํด๋์ ๊ฒ</u>์๋๋ค.

- ํฌ๊ฒ List ์ธํฐํ์ด์ค, Set ์ธํฐํ์ด์ค, Map ์ธํฐํ์ด์ค๊ฐ ์์ต๋๋ค.

- <b>List ์ธํฐํ์ด์ค</b>๋ ์์๊ฐ ์๋ ๋ชฉ๋ก์ผ๋ก, Collection์ ๋ค๋ฅธ ์ธํฐํ์ด์ค๋ค๊ณผ ๊ฐ์ฅ ํฐ ์ฐจ์ด๋ ๋ฐฐ์ด์ฒ๋ผ ์์๊ฐ ์๋ค๋ ๊ฒ์๋๋ค.

  List ์ปฌ๋ ์์ ๊ฐ์ฒด ์์ฒด๋ฅผ ์ ์ฅํ๋ ๊ฒ์ด ์๋๋ผ <u>๊ฐ์ฒด์ ๋ฒ์ง๋ฅผ ์ฐธ์กฐ</u>ํฉ๋๋ค. ์ฆ, ์ธ๋ฑ์ค๋ง๋ค ๊ฐ์ฒด์ ๋ฒ์ง์ฃผ์๊ฐ ๋ค์ด์์ต๋๋ค. ๋์ผํ ๊ฐ์ฒด๋ฅผ <u>์ค๋ณต ์ ์ฅํ  ์ ์๋๋ฐ</u>, ์ด ๊ฒฝ์ฐ ๋์ผํ ๋ฒ์ง๊ฐ ์ฐธ์กฐ๋๊ณ  null์ด ์ ์ฅ๋  ๊ฒฝ์ฐ์๋ ํด๋น ์ธ๋ฑ์ค๋ ๊ฐ์ฒด๋ฅผ ์ฐธ์กฐํ์ง ์์ต๋๋ค.

- <b>Set ์ธํฐํ์ด์ค</b>๋ <u>์์๊ฐ ์๋ ๋ฐ์ดํฐ ์งํฉ</u>์ด๊ณ , <u>๋ฐ์ดํฐ ์ค๋ณต์ ํ์ฉํ์ง ์์ต๋๋ค.</u>

- <b>Map ์ธํฐํ์ด์ค</b>๋ <u>ํค(key)์ ๊ฐ(value) ์(pair)</u>๋ก ๊ตฌ์ฑ๋ Entry ๊ฐ์ฒด๋ฅผ ์ ์ฅํ๋ ๊ตฌ์กฐ๋ฅผ ๊ฐ์ง๊ณ  ์์ต๋๋ค.

  ํค(key)๋ ์ค๋ณต ์ ์ฅ๋  ์ ์์ง๋ง, ๊ฐ์ ์ค๋ณต ์ ์ฅ๋  ์ ์์ต๋๋ค. ๋ง์ฝ ๊ธฐ์กด์ ์ ์ฅ๋ ํค์ ๋์ผํ ํค๋ก ๊ฐ์ ์ ์ฅํ๋ฉด ๊ธฐ์กด์ ๊ฐ์ ์์ด์ง๊ณ , ์๋ก์ด ๊ฐ์ผ๋ก ๋์น๋ฉ๋๋ค.

![](./src/collection.png)

<br>

#### ๐ก ArrayList์ LinkedList์ ์ฐจ์ด๋ ๋ฌด์์ธ๊ฐ์

- ๋ ๋ค List ์ธํฐํ์ด์ค์ ๊ตฌํ์ฒด์๋๋ค.

- <b>ArrayList</b>๋ <u>์ค๋ณต์ ํ์ฉํ๊ณ  ์์๋ฅผ ์ ์งํ๋ฉฐ ์ธ๋ฑ์ค๋ก ์์๋ค์ ๊ด๋ฆฌ</u>ํ๋ค๋ ์ ์์ ๋ฐฐ์ด๊ณผ ์๋นํ ์ ์ฌํฉ๋๋ค.

  ์ถ๊ฐํ์ ๋, ๋ฐฐ์ด์ด ๋์ ์ผ๋ก ๋์ด๋๋ ๊ฒ์ด ์๋๋ผ ์ฉ๋์ด ๊ฝ ์ฐผ์ ๊ฒฝ์ฐ, ๋ ํฐ ์ฉ๋์ ๋ฐฐ์ด์ ๋ง๋ค์ด ์ฎ๊ธฐ๋ ์์์ ํฉ๋๋ค.

- <b>LinkedList</b>๋ <u>๋ด๋ถ์ ์ผ๋ก ์๋ฐฉํฅ์ ์ฐ๊ฒฐ ๋ฆฌ์คํธ๋ก ๊ตฌ์ฑ</u>๋์ด ์์ด์ ์ฐธ์กฐํ๋ ค๋ ์์์ ๋ฐ๋ผ ์ฒ์๋ถํฐ ์๋ฐฉํฅ์ผ๋ก ๋๋ ์ญ์์ผ๋ก ์ํํ  ์ ์์ต๋๋ค.

- <u>์์ฐจ์ ์ผ๋ก ์ถ๊ฐ/์ญ์ ํ</u>๋ ๊ฒฝ์ฐ์๋ <u>ArrayList๊ฐ LinkedList๋ณด๋ค ๋น ๋ฆ๋๋ค.</u>

  ์์ฐจ์ ์ผ๋ก ์ญ์ ํ๋ค๋ ๊ฒ์ ๋ง์ง๋ง ๋ฐ์ดํฐ๋ถํฐ ์ญ์ ํ  ๊ฒฝ์ฐ ๊ฐ ์์๋ค์ ์ฌ๋ฐฐ์น๊ฐ ํ์ํ์ง ์๊ธฐ ๋๋ฌธ์ ์๋นํ ๋น ๋ฆ๋๋ค.

- <u>์ค๊ฐ ๋ฐ์ดํฐ๋ฅผ ์ถ๊ฐ/์ญ์ </u>ํ๋ ๊ฒฝ์ฐ์๋ <u>LinkedList๊ฐ ArrayList๋ณด๋ค ๋น ๋ฆ๋๋ค.</u>

  ์ค๊ฐ ์์๋ฅผ ์ถ๊ฐ, ์ญ์ ํ๋ ๊ฒฝ์ฐ, LinkedList๋ ๊ฐ ์์๊ฐ์ ์ฐ๊ฒฐ๋ง ๋ณ๊ฒฝํด์ฃผ๋ฉด ๋๊ธฐ ๋๋ฌธ์ ์ฒ๋ฆฌ ์๋๊ฐ ์๋นํ ๋น ๋ฆ๋๋ค. ๋ฐ๋ฉด์ ArrayList๋ ๊ฐ ์์๋ค์ ์ฌ๋ฐฐ์นํด ์ถ๊ฐ ๊ณต๊ฐ์ ํ๋ณดํ๊ฑฐ๋ ๋น ๊ณต๊ฐ์ ์ฑ์์ผ ํ๊ธฐ ๋๋ฌธ์ ์ฒ๋ฆฌ ์๋๊ฐ ๋๋ฆฝ๋๋ค.

<br>

#### ๐ก this ํค์๋๋ ์ธ์  ์ฌ์ฉ๋๋์?

- <b>this</b>๋ <u>์๊ธฐ ์์ ์ ์์ฑ์ ๊ฐ๋ฆฌํค๋ ๊ฒ</u>์ผ๋ก,

  ์ฃผ๋ก ์์ฑ์์ ๋ฉ์๋์ ๋งค๊ฐ๋ณ์ ์ด๋ฆ์ด ํ๋์ ๋น์ทํ๊ฑฐ๋ ๊ฐ์ ๊ฒฝ์ฐ, ์ธ์คํด์ค ๋ฉค๋ฒ์ธ ํ๋์์ ๋ช์ํ๊ณ ์ ํ  ๋ ์ฌ์ฉ๋ฉ๋๋ค.

- this๋ ๋ฉ์๋ ๋ด์์ ์ฌ์ฉํ๊ฑฐ๋, ๊ฐ์ฒด ์์ฑ์ ๋ด์์ ๋ค๋ฅธ ์์ฑ์๋ฅผ ํธ์ถํ  ๋ ์ฌ์ฉํฉ๋๋ค.

<br>

<br>

---

**[์ฐธ๊ณ ]**

[JVM ๊ตฌ์กฐ](https://velog.io/@litien/JVM-%EA%B5%AC%EC%A1%B0)

[JVM ๊ตฌ์กฐ](https://velog.io/@hono2030/JVM%EC%9D%98-%EA%B5%AC%EC%A1%B0)

[๊ฐ๋น์ง ์ฝ๋ ํฐ](https://velog.io/@litien/%EA%B0%80%EB%B9%84%EC%A7%80-%EC%BB%AC%EB%A0%89%ED%84%B0GC)

[Garbage Collection](https://mangkyu.tistory.com/118)

[JAVA Garbage Collection](https://d2.naver.com/helloworld/1329)

[JAVA SE์ EE์ ์ฐจ์ด](https://doozi316.github.io/java/2020/07/01/WEB20/)

[๊ธฐ๋ณธํ๊ณผ ์ฐธ์กฐํ & ==์ Equals()์ ์ฐจ์ด](https://shyvana.tistory.com/12)

[์ฐธ์กฐํ ๋ณ์](https://colossus-java-practice.tistory.com/7)

[์ ๊ทผ ์ ์ด์](http://tcpschool.com/java/java_modifier_accessModifier)

[static๊ณผ non-static์ ์ฐจ์ด](https://lifejusik1004.tistory.com/entry/JAVA-static-%EA%B3%BC-non-static-%EC%9D%98-%EC%B0%A8%EC%9D%B4)

[ํด๋์ค(static) ๋ณ์์ ์ธ์คํด์ค(non-static) ๋ณ์](https://sujinhope.github.io/2021/03/03/Java-%ED%81%B4%EB%9E%98%EC%8A%A4%EB%B3%80%EC%88%98,-%EC%9D%B8%EC%8A%A4%ED%84%B4%EC%8A%A4-%EB%B3%80%EC%88%98-%EC%B0%A8%EC%9D%B4(Static%EB%B3%80%EC%88%98%EC%99%80-Non-Static%EB%B3%80%EC%88%98).html)

[๋ฉ์ธ ๋ฉ์๋๊ฐ public static void์ธ ์ด์ ](https://jaehoney.tistory.com/37)

[final ํค์๋](https://hbase.tistory.com/151)

[์ ๋ค๋ฆญ](http://tcpschool.com/java/java_generic_concept)

[Call By Value์ Call By Reference](https://devlog-wjdrbs96.tistory.com/44)

[Call By Value, Call By Reference](https://velog.io/@ahnick/Java-Call-by-Value-Call-by-Reference)

[์ถ์ ํด๋์ค์ ์ธํฐํ์ด์ค์ ์ฐจ์ด](https://velog.io/@new_wisdom/Java-%EC%B6%94%EC%83%81-%ED%81%B4%EB%9E%98%EC%8A%A4%EC%99%80-%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4%EC%9D%98-%EC%B0%A8%EC%9D%B4)

[์ถ์ ํด๋์ค์ ์ธํฐํ์ด์ค์ ์ฐจ์ด](https://haenny.tistory.com/162)

[Reflection์ด๋?](https://velog.io/@yeon/Reflection%EC%9D%B4%EB%9E%80)

[StringBuffer vs String Builder vs String](https://madplay.github.io/post/difference-between-string-stringbuilder-and-stringbuffer-in-java)

[Java 8](https://medium.com/@inhyuck/java-8%EC%97%90-%EC%B6%94%EA%B0%80%EB%90%9C-%EA%B2%83%EB%93%A4-8c66023cbbae)

[Java ๋๋ค(lambda)](https://girawhale.tistory.com/124)

[์์ธ ์ฒ๋ฆฌ](https://mangkyu.tistory.com/152)

[Collection](https://hoon26.tistory.com/25)

[ArrayList์ LinkedList์ ์ฐจ์ด](https://devlog-wjdrbs96.tistory.com/64)

[this](https://fora.tistory.com/16)
