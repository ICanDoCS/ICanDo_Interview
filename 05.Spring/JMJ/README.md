# Part 05. Spring

#### π‘ JDBCλ λ¬΄μμΈκ°μ?

**JDBC**(Java Database Connectivity)λ μλ°μμ λ°μ΄ν°λ² μ΄μ€μ μ μν  μ μλλ‘ νλ μλ° APIμ΄λ€. **JDBC**λ λ°μ΄ν°λ² μ΄μ€μμ μλ£λ₯Ό μΏΌλ¦¬νκ±°λ μλ°μ΄νΈνλ λ°©λ²μ μ κ³΅νλ€.

**μμ ν λ²μ :** JDBC 4.3 / 2017λ 9μ 21μΌ

**μ’λ₯:** λ°μ΄ν° μ κ·Ό API



#### π‘ Servletμ΄λ λ¬΄μμΈκ°μ?

> - ν΄λΌμ΄μΈνΈμ μμ²­μ μ²λ¦¬νκ³ , κ·Έ κ²°κ³Όλ₯Ό λ°ννλ Servlet ν΄λμ€μ κ΅¬ν κ·μΉμ μ§ν¨ μλ° μΉ νλ‘κ·Έλλ° κΈ°μ 
> - Javaλ₯Ό μΉμ΄νλ¦¬μΌμ΄μμ μ‘°κΈ λ κ°λ°νκΈ° μ½κ² νκΈ° μν΄ λ§λ  API(λΌμ΄λΈλ¬λ¦¬, ν΄λμ€ λ€)μ΄λ©° μ΄ κ·μ½μ λ§λ λΌμ΄λΈλ¬λ¦¬λ ν΄λμ€λ€μ μμ λ° κ΅¬ννμ¬ λ§λ  ν΄λμ€λ€μ μλΈλ¦Ώμ΄λΌκ³  νλ€.

- `Servlet`μ μλ² μͺ½μμ μ€νλλ©΄μ ν΄λΌμ΄μΈνΈμ μμ²­μ λ°λΌ λμ μΌλ‘ μλΉμ€λ₯Ό μ κ³΅νλ `μλ° ν΄λμ€`μ΄λ€.

- λμμ μΌλ‘ μ€νν  μ μμΌλ©°, ν°μΊ£κ³Ό κ°μ `JSP/Servlet μ»¨νμ΄λ`μμλ§ μ€ν κ°λ₯νλ©°, μ»¨νμ΄λ λλ¦½μ μΌλ‘ μ€νλλ€.

- μλΈλ¦Ώμ μλ²μμ μ€νλλ€κ° μΉ λΈλΌμ°μ μμ μμ²­μ νλ©΄ ν΄λΉ κΈ°λ₯μ μν ν, μΉ λΈλΌμ°μ μ κ²°κ³Όλ₯Ό μ μ‘νλ€.

  #### νΉμ§

  - ν΄λΌμ΄μΈνΈμ μμ²­μ λν΄ λμ μΌλ‘ μλνλ μΉ μ΄νλ¦¬μΌμ΄μ μ»΄ν¬λνΈ
  - Java Threadλ₯Ό μ΄μ©νμ¬ λμνλ€!
  - MVC ν¨ν΄μμ Controllerλ‘ μ΄μ©νλ€.

  

#### π‘ JSPλ λ¬΄μμΈκ°?

> JSP (Java Server Page)

- μΉ μ¬μ©μκ° ν­λ°μ μΌλ‘ μ¦κ°νκ³ , μΉ νμ΄μ§λ λ³΅μ‘ν΄μ§κ³  κ³ λνλ¨μ λ°λΌ, κ°λ°μμ λμμ΄λμ λΆμμ΄ μΌμ΄λκΈ° μμνμλ€.
- λμμ΄λκ° μλ°μ μλΈλ¦Ώμ μ½λμ μ΅μνμ§ μμ νλ©΄ κΈ°λ₯ κ΅¬νμ λΆνΈν¨μ΄ λ§μλ€.
- μλΈλ¦Ώμ κΈ°λ₯ μ€ νλ©΄ λΆλΆμ λμμ΄λκ° μ½κ² μμνκΈ° μν΄ `JSP`κ° λ±μ₯νμλ€.
- JSP νμΌμμλ HTMLλ‘ μμ±λ λ¬Έμ μμ `<% %>` , `<%= %>` λ±μ λ°κ΅¬λ μμ μλ°μ½λλ₯Ό μ½μν  μ μλ€.
- `Java μ»¨νμ΄λ`λ JSPνμΌμ HTMLμ½λμ μλ°μ½λλ₯Ό λΆλ¦¬νμ¬ `classνμΌ`μ λ§λ€κ³  μ€ννλ€.
- javaμΈμ΄ κΈ°λ°μΌλ‘ **λμ μΈ μΉ νμ΄μ§**λ₯Ό κ΅¬μ±ν  μ μλ€



### Servletκ³Ό JSPμ μ°¨μ΄
#### Servlet
- Java μ½λ μμ HTML μ½λ (νλμ ν΄λμ€)
- data processing(Controller)μ μ’λ€. μ¦ DBμμ ν΅μ , Business Logic νΈμΆ, λ°μ΄ν°λ₯Ό μ½κ³  νμΈνλ μμ λ±μ μ μ©νλ€.
- Servletμ΄ μμ λ κ²½μ° Java μ½λλ₯Ό μ»΄νμΌ(.class νμΌ μμ±)ν ν λμ μΈ νμ΄μ§λ₯Ό μ²λ¦¬νκΈ° λλ¬Έμ μ μ²΄ μ½λλ₯Ό μλ°μ΄νΈνκ³  λ€μ μ»΄νμΌν ν μ¬λ°°ν¬νλ μμμ΄ νμνλ€. (κ°λ° μμ°μ± μ ν)

#### JSP
- HTML μ½λ μμ Java μ½λ

- presentation(View)μ μ’λ€. μ¦ μμ²­ κ²°κ³Όλ₯Ό λνλ΄λ HTML μμ±νλλ° μ μ©νλ€.

- JSPκ° μμ λ κ²½μ° μ¬λ°°ν¬ν  νμκ° μμ΄ WASκ° μμμ μ²λ¦¬νλ€. (μ¬μ΄ λ°°ν¬)

  

#### π‘ pojoλ λ¬΄μμΈκ°μ?

> POJO (Plain Old Java Object), λ³Έλ μλ°μ μ₯μ μ μ΄λ¦¬λ 'μ€λλ' λ°©μμ 'μμν' μλ°κ°μ²΄
>
> μ§μ ν POJOλ κ°μ²΄μ§ν₯μ μΈ μλ¦¬μ μΆ©μ€νλ©΄μ, νκ²½κ³Ό κΈ°μ μ μ’μλμ§ μκ³  νμμ λ°λΌ μ¬νμ©λ  μ μλ λ°©μμΌλ‘ μ€κ³λ μ€λΈμ νΈλ₯Ό λ§νλ€.

##### POJOλ₯Ό μ λ¦¬νμλ©΄,

- νΉμ  κ·μ½(contract)μ μ’μλμ§ μλλ€. (Java μΈμ΄μ κΌ­ νμν API μΈμ μ’μλμ§ μλλ€.)
- νΉμ  νκ²½μ μ’μλμ§ μλλ€.
- κ°μ²΄μ§ν₯μλ¦¬μ μΆ©μ€ν΄μΌ νλ€.

##### POJOλ₯Ό μ¬μ©νλ μ΄μ 

- μ½λμ κ°κ²°ν¨ (λΉμ¦λμ€ λ‘μ§κ³Ό νΉμ  νκ²½/low λ λ²¨ μ’μμ μΈ μ½λλ₯Ό λΆλ¦¬νλ―λ‘ λ¨μνλ€.)
- μλν νμ€νΈμ μ λ¦¬ (νκ²½ μ’μμ μΈ μ½λλ μλν νμ€νΈκ° μ΄λ ΅μ§λ§, POJOλ νμ€νΈκ° λ§€μ° μ μ°νλ€.
- κ°μ²΄μ§ν₯μ  μ€κ³μ μμ λ‘μ΄ μ¬μ©

##### POJO νλ μμν¬ 

- **POJOλ₯Ό μ΄μ©ν μ νλ¦¬μΌμ΄μ κ°λ°μ΄ κ°μ§ νΉμ§κ³Ό μ₯μ μ κ·Έλλ‘ μ΄λ¦¬λ©΄μ EJBμμ μ κ³΅νλ μν°νλΌμ΄μ¦ μλΉμ€μ κΈ°μ μ κ·Έλλ‘ μ¬μ©ν  μ μλλ‘ λμμ£Όλ νλ μμν¬**

###### **μ€νλ§ νλ μμν¬**

- μ€νλ§ : POJO νλ μμν¬ μ€ νλμ΄λ©°, μλ° μ νλ¦¬μΌμ΄μ κ°λ°μ μν ν¬κ΄μ μΈ μΈνΈλΌ μ€νΈλ­μ²λ₯Ό μ κ³΅νλ μλ° νλ«νΌμ΄λ€. 

- μ€νλ§μ μ¬μ©νλ©΄ POJOλ‘ μ΄νλ¦¬μΌμ΄μμ λ§λ€κ³  μν°νλΌμ΄μ¦ μλΉμ€λ₯Ό λΉμΉ¨ν¬μ μΌλ‘ POJOμ μ μ©ν  μ μλ€. 



#### π‘ Spring AOPλ?

- **AOP**λ **Aspect Oriented Programming**μ μ½μλ‘ **κ΄μ  μ§ν₯ νλ‘κ·Έλλ°**
- κ΄μ  μ§ν₯μ μ½κ² λ§ν΄ **μ΄λ€ λ‘μ§μ κΈ°μ€μΌλ‘ ν΅μ¬μ μΈ κ΄μ , λΆκ°μ μΈ κ΄μ μΌλ‘ λλμ΄μ λ³΄κ³  κ·Έ κ΄μ μ κΈ°μ€μΌλ‘ κ°κ° λͺ¨λννκ² λ€λ κ²μ΄λ€**. (λͺ¨λνλ μ΄λ€ κ³΅ν΅λ λ‘μ§μ΄λ κΈ°λ₯μ νλμ λ¨μλ‘ λ¬Άλ κ²μ λ§νλ€.)
- μ) ν΅μ¬μ μΈ κ΄μ μ κ²°κ΅­ μ°λ¦¬κ° μ μ©νκ³ μ νλ ν΅μ¬ λΉμ¦λμ€ λ‘μ§μ΄ λλ€. λν λΆκ°μ μΈ κ΄μ μ ν΅μ¬ λ‘μ§μ μ€ννκΈ° μν΄μ νν΄μ§λ λ°μ΄ν°λ² μ΄μ€ μ°κ²°, λ‘κΉ, νμΌ μμΆλ ₯ λ±μ μλ‘ λ€ μ μλ€.
- **AOP**μμ κ° κ΄μ μ κΈ°μ€μΌλ‘ λ‘μ§μ λͺ¨λννλ€λ κ²μ μ½λλ€μ λΆλΆμ μΌλ‘ λλμ΄μ λͺ¨λννκ² λ€λ μλ―Έλ€. μ΄λ, μμ€ μ½λμμμ λ€λ₯Έ λΆλΆμ κ³μ λ°λ³΅ν΄μ μ°λ μ½λλ€μ λ°κ²¬ν  μ μλ λ° μ΄κ²μ **ν©μ΄μ§ κ΄μ¬μ¬ (Crosscutting Concerns)**λΌ λΆλ₯Έλ€. 

<img src="image/aop.png" style="zoom:30%;" />

- μμ κ°μ΄ ν©μ΄μ§ κ΄μ¬μ¬λ₯Ό **Aspectλ‘ λͺ¨λννκ³  ν΅μ¬μ μΈ λΉμ¦λμ€ λ‘μ§μμ λΆλ¦¬νμ¬ μ¬μ¬μ©νκ² λ€λ κ²μ΄ AOPμ μ·¨μ§**λ€.

  

**| AOP μ£Όμ κ°λ**

- Aspect : μμμ μ€λͺν ν©μ΄μ§ κ΄μ¬μ¬λ₯Ό λͺ¨λν ν κ². μ£Όλ‘ λΆκ°κΈ°λ₯μ λͺ¨λνν¨.
- Target : Aspectλ₯Ό μ μ©νλ κ³³ (ν΄λμ€, λ©μλ .. )
- Advice : μ€μ§μ μΌλ‘ μ΄λ€ μΌμ ν΄μΌν  μ§μ λν κ², μ€μ§μ μΈ λΆκ°κΈ°λ₯μ λ΄μ κ΅¬νμ²΄
- JointPoint : Adviceκ° μ μ©λ  μμΉ, λΌμ΄λ€ μ μλ μ§μ . λ©μλ μ§μ μ§μ , μμ±μ νΈμΆ μμ , νλμμ κ°μ κΊΌλ΄μ¬ λ λ± λ€μν μμ μ μ μ©κ°λ₯
- PointCut : JointPointμ μμΈν μ€νμ μ μν κ². 'Aλ λ©μλμ μ§μ μμ μ νΈμΆν  κ²'κ³Ό κ°μ΄ λμ± κ΅¬μ²΄μ μΌλ‘ Adviceκ° μ€νλ  μ§μ μ μ ν  μ μμ



**| μ€νλ§ AOP νΉμ§**

- νλ‘μ ν¨ν΄ κΈ°λ°μ AOP κ΅¬νμ²΄, νλ‘μ κ°μ²΄λ₯Ό μ°λ μ΄μ λ μ κ·Ό μ μ΄ λ° λΆκ°κΈ°λ₯μ μΆκ°νκΈ° μν΄μμ
- μ€νλ§ λΉμλ§ AOPλ₯Ό μ μ© κ°λ₯
- λͺ¨λ  AOP κΈ°λ₯μ μ κ³΅νλ κ²μ΄ μλ μ€νλ§ IoCμ μ°λνμ¬ μν°νλΌμ΄μ¦ μ νλ¦¬μΌμ΄μμμ κ°μ₯ νν λ¬Έμ (μ€λ³΅μ½λ, νλ‘μ ν΄λμ€ μμ±μ λ²κ±°λ‘μ, κ°μ²΄λ€ κ° κ΄κ³ λ³΅μ‘λ μ¦κ° ...)μ λν ν΄κ²°μ±μ μ§μνλ κ²μ΄ λͺ©μ 



μΆμ²: https://engkimbs.tistory.com/746 



#### π‘ Spring DIλ?

`DI(Dependency Injection)`λ **μ€νλ§μ΄ λ€λ₯Έ νλ μμν¬μ μ°¨λ³νλμ΄ μ κ³΅νλ μμ‘΄ κ΄κ³ μ£Όμ κΈ°λ₯**μΌλ‘,
**κ°μ²΄λ₯Ό μ§μ  μμ±νλ κ² μλλΌ μΈλΆμμ μμ±ν ν μ£Όμ μμΌμ£Όλ λ°©μ**μ΄λ€.

**DI(μμ‘΄μ± μ£Όμ)λ₯Ό ν΅ν΄μ λͺ¨λ κ°μ κ²°ν©λκ° λ?μμ§κ³  μ μ°μ±μ΄ λμμ§λ€.**



<img src="image/DI1.png" style="zoom:30%;" />

μ²«λ²μ§Έ λ°©λ²μ Aκ°μ²΄κ° Bμ Cκ°μ²΄λ₯Ό New μμ±μλ₯Ό ν΅ν΄μ μ§μ  μμ±νλ λ°©λ²μ΄κ³ ,

λλ²μ§Έ λ°©λ²μ **μΈλΆμμ μμ± λ κ°μ²΄λ₯Ό setter()λ₯Ό ν΅ν΄ μ¬μ©νλ λ°©λ²**μ΄λ€.

μ΄λ¬ν λλ²μ§Έ λ°©μμ΄ μμ‘΄μ± μ£Όμμ μμμΈλ°,
`A κ°μ²΄`μμ **`B, Cκ°μ²΄`λ₯Ό μ¬μ©(μμ‘΄)ν  λ** `A κ°μ²΄`μμ **μ§μ  μμ± νλ κ²μ΄ μλλΌ** **`μΈλΆ(IOCμ»¨νμ΄λ)`μμ μμ±λ `B, Cκ°μ²΄`λ₯Ό μ‘°λ¦½(μ£Όμ)μμΌ `setter` νΉμ `μμ±μ`λ₯Ό ν΅ν΄ μ¬μ©νλ λ°©μ**μ΄λ€.



<img src="image/DI2.png" style="zoom:33%;" />

**μ€νλ§μμλ κ°μ²΄λ₯Ό `Bean`**μ΄λΌκ³  λΆλ₯΄λ©°, νλ‘μ νΈκ° μ€νλ λ μ¬μ©μκ° BeanμΌλ‘ κ΄λ¦¬νλ κ°μ²΄λ€μ μμ±κ³Ό μλ©Έμ κ΄λ ¨λ μμμ μλμ μΌλ‘ μνν΄μ£Όλλ° κ°μ²΄κ° μμ±λλ κ³³μ μ€νλ§μμλ Bean μ»¨νμ΄λλΌκ³  λΆλ₯Έλ€.



#### π‘ Spring IOCλ λ¬΄μμΈκ°?

`IoC(Inversion of Control)`λ "μ μ΄μ μ­μ " μ΄λΌλ μλ―Έλ‘, λ§ κ·Έλλ‘ **λ©μλλ κ°μ²΄μ νΈμΆμμμ κ°λ°μκ° κ²°μ νλ κ²μ΄ μλλΌ, μΈλΆμμ κ²°μ λλ κ²μ μλ―Έ**νλ€.



`IoC`λ **μ μ΄μ μ­μ μ΄λΌκ³  λ§νλ©°, κ°λ¨ν λ§ν΄ "μ μ΄μ νλ¦μ λ°κΎΌλ€"**λΌκ³  νλ€.

κ°μ²΄μ **μμ‘΄μ±μ μ­μ μμΌ κ°μ²΄ κ°μ κ²°ν©λλ₯Ό μ€μ΄κ³  μ μ°ν μ½λλ₯Ό μμ±**ν  μ μκ² νμ¬ **κ°λμ± λ° μ½λ μ€λ³΅, μ μ§ λ³΄μλ₯Ό νΈνκ²** ν  μ μκ² νλ€.

κΈ°μ‘΄μλ λ€μκ³Ό μμλ‘ κ°μ²΄κ° λ§λ€μ΄μ§κ³  μ€νλμλ€.

1. κ°μ²΄ μμ±
2. μμ‘΄μ± κ°μ²΄ μμ±
   *ν΄λμ€ λ΄λΆμμ μμ±*
3. μμ‘΄μ± κ°μ²΄ λ©μλ νΈμΆ

νμ§λ§, μ€νλ§μμλ λ€μκ³Ό κ°μ μμλ‘ κ°μ²΄κ° λ§λ€μ΄μ§κ³  μ€νλλ€.

1. κ°μ²΄ μμ±
2. μμ‘΄μ± κ°μ²΄ μ£Όμ
   *μ€μ€λ‘κ° λ§λλκ²μ΄ μλλΌ μ μ΄κΆμ **μ€νλ§μκ² μμνμ¬ μ€νλ§μ΄ λ§λ€μ΄λμ κ°μ²΄λ₯Ό μ£Όμ**νλ€.*
3. μμ‘΄μ± κ°μ²΄ λ©μλ νΈμΆ

**μ€νλ§μ΄ λͺ¨λ  μμ‘΄μ± κ°μ²΄λ₯Ό μ€νλ§μ΄ μ€νλ λ λ€ λ§λ€μ΄μ£Όκ³  νμνκ³³μ μ£Όμ**μμΌμ€μΌλ‘μ¨ **Beanλ€μ `μ±κΈν΄ ν¨ν΄`μ νΉμ§**μ κ°μ§λ©°,

**μ μ΄μ νλ¦μ μ¬μ©μκ° μ»¨νΈλ‘€ νλ κ²μ΄ μλλΌ μ€νλ§μκ² λ§‘κ²¨ μμμ μ²λ¦¬**νκ² λλ€.



[μΆμ²] https://velog.io/@gillog/Spring-DIDependency-Injection



#### π‘ Spring MVC νλ¦μ λν μ€λͺ

μΉ μ΄νλ¦¬μΌμ΄μμ ν¬κ² **MVC** ν¨ν΄μ λ°λ₯΄κ² λλ©° **Model, View, Controller**λ‘ λλκ² λλ€. 

- Model : DBμ μνΈμμ©νλ©° λΉμ¦λμ€ λ‘μ§μ μ²λ¦¬νλ λͺ¨λ 
- View : Clientμκ² λ³΄μ¬μ§λ κ²°κ³Όνλ©΄μ λ°ννλ λͺ¨λ
- Controller : Client μμ²­μ΄ λ€μ΄μμ λ κ·Έ μλ ₯μ μ²λ¦¬νκ³  μ΄λ€ λ‘μ§μ μ€νμν¬ κ²μΈμ§ μ μ΄νλ λͺ¨λ

<img src="image/mvc.png" style="zoom:40%;" />

###### μΆμ² : λΆμ€νΈμ½μ€(https://www.edwith.org/boostcourse-web/lecture/16762/)

- - Model μ 'λ°μ΄ν°' λμμΈμ λ΄λΉνλ€.
    - ex. μν λͺ©λ‘, μ£Όλ¬Έ λ΄μ­ λ±
  - View λ 'μ€μ λ‘ λ λλ§λμ΄ λ³΄μ΄λ νμ΄μ§' λ₯Ό λ΄λΉνλ€.
    - ex. `.JSP` νμΌλ€μ΄ μ¬κΈ°μ ν΄λΉλλ€.
  - Controller λ μ¬μ©μμ μμ²­μ λ°κ³ , μλ΅μ μ£Όλ λ‘μ§μ λ΄λΉνλ€.
    - ex. GET λ±μ uri λ§€νμ΄ μ¬κΈ°μ ν΄λΉλλ€.
- Spring MVC λͺ¨λμ μ¬μ©νμ¬, λ°±μλ νλ‘κ·Έλλ°μ κΈ°λ³Έ νλ μμν¬λ₯Ό μ‘λλ€.
  - Web μλ²μ νΉνλμ΄ λ§λ€μ΄μ§ λͺ¨λμ΄λΌ, κ°λ°μκ° ν΄μΌν  μμ­μ λ μ κ² λ§λ€μ΄μ€λ€.
  - μ¦ κΈ°μ‘΄μ Spring λ³΄λ€ λ κΉλνκ³  κ°νΈνκ² κ°λ° κ°λ₯.
- λ³λ€λ₯Έ λ§μ΄ μμΌλ©΄ MVC Model 2 μν€νμ²λ₯Ό μ¬μ©νλ κ²μΌλ‘ μκ°νλ€.



#### π‘ Spring MVC1κ³Ό MVC2μ μ°¨μ΄μ μ?

##### MVC1

<img src="image/mvc1.png" style="zoom:50%;" />

MVC1 ν¨ν΄μ κ²½μ° Viewμ Controllerλ₯Ό λͺ¨λ JSPκ° λ΄λΉνλ ννλ₯Ό κ°μ§λλ€. μ¦ JSP νλλ‘ μ μ μ μμ²­μ λ°κ³  μλ΅μ μ²λ¦¬νλ―λ‘ **κ΅¬ν λμ΄λλ μ½μ΅λλ€.**

λ¨μν νλ‘μ νΈμλ κ΄μ°?κ² μ§λ§ λ΄μ©μ΄ λ³΅μ‘νκ³  κ±°λν΄μ§μλ‘ μ΄ ν¨ν΄μ νμ μμ΅λλ€. **JSP νλμμ MVC κ° λͺ¨λ μ΄λ£¨μ΄μ§λ€λ³΄λ μ¬μ¬μ©μ±λ λ§€μ° λ¨μ΄μ§κ³ , μ½κΈ°λ νλ€μ΄μ§λλ€.** μ¦ **μ μ§λ³΄μμ μμ΄μ λ¬Έμ κ° λ°μν©λλ€.**



##### MVC2

<img src="image/mvc2.png" style="zoom:50%;" />

MVC2 ν¨ν΄μ λλ¦¬ νμ€μΌλ‘ μ¬μ©λλ ν¨ν΄μλλ€. **μμ²­μ νλμ μ»¨νΈλ‘€λ¬(Servlet)κ° λ¨Όμ  λ°μ΅λλ€.** μ¦ MVC1κ³Όλ λ€λ₯΄κ² **Controller, Viewκ° λΆλ¦¬λμ΄ μμ΅λλ€.** λ°λΌμ μ­ν μ΄ λΆλ¦¬λμ΄ MVC1ν¨ν΄μμμ λ¨μ μ λ³΄μν  μ μμ΅λλ€. κ·Έλ¬λ―λ‘ κ°λ°μλ M, V, C μ€μμ μμ ν΄μΌ ν  λΆλΆμ΄ μλ€λ©΄, κ·Έκ²λ§ κΊΌλ΄μ΄ μμ νλ©΄ λ©λλ€. λ°λΌμ μ μ§λ³΄μμ μμ΄μλ ν° μ΄μ μ κ°μ§λλ€.

MV2λ MVC1 ν¨ν΄λ³΄λ€ κ΅¬μ‘°κ° λ³΅μ‘ν΄μ§ μ μμ§λ§, κ°λ°μκ° μ΄λ¬ν μΈλΆμ μΈ κ΅¬μ±κΉμ§ μ κ²½μ°μ§ μμ μ μλλ‘ **κ°μ’ νλ μμν¬λ€μ΄ μ§κΈκΉμ§ μ λ°μ λμ΄ μμ΅λλ€.** κ·Έ μ€μμ λνμ μΈ κ²μ΄ λ°λ‘ **μ€νλ§ νλ μμν¬**μλλ€.



##### Spring & MVC2

<img src="image/mvc2_spring.png" style="zoom:40%;" />

[μΆμ²] https://chanhuiseok.github.io/posts/spring-3/



#### π‘ Springκ³Ό Spring Bootμ μ°¨μ΄μ μ?

- **μ€νλ§** νλ μμν¬λ κΈ°λ₯μ΄ λ§μλ§νΌ νκ²½μ€μ μ΄ λ³΅μ‘ν νΈμ΄λ€. μ΄μ μ΄λ €μμ λλΌλ μ¬μ©μλ€μ μν΄ λμ¨ κ²μ΄ λ°λ‘ **μ€νλ§ λΆνΈ**λ€. 

- **μ€νλ§ λΆνΈ**λ **μ€νλ§** νλ μμν¬λ₯Ό μ¬μ©νκΈ° μν μ€μ **μ** λ§μ λΆλΆμ μλννμ¬ μ¬μ©μκ° μ λ§ νΈνκ² **μ€νλ§**μ νμ©ν  μ μλλ‘ λλλ€.

  

#### π‘ DAOμ DTOμ μ°¨μ΄μ μ?

**DAO**

\- Data Access Object, λ°μ΄ν°λ² μ΄μ€μ dataμ μ κ·ΌνκΈ° μν κ°μ²΄

\- DAM(Data Access Module)κ³Ό μ μ¬ν μ­ν 

\- DBμ κ·Ό λ‘μ§κ³Ό λΉμ¦λμ€ λ‘μ§μ κ΅¬λΆνκΈ° μν¨

-> DAOμ κ²½μ°λ DBμ μ°κ²°ν  Connection κΉμ§ μ€μ λμ΄ μλ κ²½μ°κ° λ§μ. κ·Έλμ νμ¬ λ§μ΄ μ°μ΄λ Mybatis λ±μ μ¬μ©ν  κ²½μ° μ»€λ₯μνκΉμ§ μ κ³΅λκ³  μκΈ° λλ¬Έμ DAOλ₯Ό λ³λλ‘ λ§λλ κ²½μ°λ λλ¬Όλ€.



**DTO**

\- Data Transfer Object, κ³μΈ΅κ° λ°μ΄ν° κ΅νμ μν μλ° beans

\- κ° κ³μΈ΅κ° λ°μ΄ν° κ΅νμ μν κ°μ²΄

\- λ‘μ§μ κ°κ³  μμ§ μλ μμν λ°μ΄ν° κ°μ²΄μ΄λ©°, getter/setter λ©μλλ§ λ³΄μ ν ν΄λμ€



#### π‘ Mybatisλ λ¬΄μμΈκ°?

- Mybatisλ μλ° μ€λΈμ νΈμ SQLμ¬μ΄μ μλ λ§€ν κΈ°λ₯μ μ§μνλ ORM(Object relational Mapping)νλ μμν¬μ΄λ€.

- SQLμ λ³λμ νμΌλ‘ λΆλ¦¬ν΄μ κ΄λ¦¬νκ² ν΄μ€λ€.
  Hibernateλ JAP(Java Persistence Api)μ²λΌ μλ‘μ΄ DBνλ‘κ·Έλλ° ν¨λ¬λ€μμ μ΅νμΌνλ λΆλ΄ μμ΄ SQLμ κ·Έλλ‘ μ΄μ©νλ©΄μ JDBCμ½λ μμ±μ λΆνΈν¨λ μ κ±°ν΄μ£Όκ³  λλ©μΈ κ°μ²΄λ VOκ°μ²΄λ₯Ό μ€μ¬μΌλ‘ κ°λ°μ΄ κ°λ₯νλ€λ μ₯μ μ΄ μλ€.

##### Mybatisμ νΉμ§

1. μ¬μ΄ μ κ·Όμ±κ³Ό μ½λμ κ°κ²°ν¨
   JDBCμ λͺ¨λ  κΈ°λ₯μ Mybatisκ° λλΆλΆ μ κ³΅νλ€.
   λ³΅μ‘ν JDBCμ½λλ₯Ό κ±·μ΄λ΄λ©° κΉλν μμ€μ½λλ₯Ό μ μ§ν  μ μλ€.
   μλμ μΈ νλΌλ―Έν° μ€μ κ³Ό μΏΌλ¦¬ κ²°κ³Όμ λν λ§΅ν κ΅¬λ¬Έμ μ κ±°ν  μ μλ€.

2. SQLλ¬Έκ³Ό νλ‘κ·Έλλ° μ½λμ λΆλ¦¬
   SQLμ λ³κ²½μ΄ μμ λλ§λ€ μλ° μ½λλ₯Ό μμ νκ±°λ μ»΄νμΌνμ§ μμλ λλ€.

3. λ€μν νλ‘κ·Έλλ° μΈμ΄λ‘ κ΅¬νκ°λ₯
   Java, C#, .NET, Ruby

   

#### π‘ MyBatisμ Spring JPAμ μ₯λ¨μ 

```null
> SQL Mapper

SQL Mapperλ μ§μ  SQLλ¬Έμ μμ±ν΄ DBλ₯Ό μ κ·Όνλ κ²μ΄λ€.
Mybatisκ° SQL Mapperμ ν΄λΉνλ€.

> ORM (Object Relational Mapping)

DBμ λ°μ΄ν°λ₯Ό κ°μ²΄λ‘ λ§€νμμΌ λ°μ΄ν°λ₯Ό μ κ·Όν  μ μλ κ²μ΄λ€.
ORMμ μ¬μ©νλ©΄ SQLμ μμ±νμ§ μκ³ λ λ©μλλ₯Ό μ¬μ©ν΄ λ°μ΄ν°λ₯Ό μ‘°μν  μ μλ€.
JPA, Hibernate λ±μ΄ ν΄λΉνλ€.
```



#### @ Mybatis

Javaμμλ DBμ μ κ·Όν  μ μλλ‘ **JDBC**λΌλ λΌμ΄λΈλ¬λ¦¬λ₯Ό μ κ³΅νλ€.
JDBCλ νμ΅μ΄ μ¬μμ μ²μ DB μ κ·Όμ λ°°μΈ λ μμ£Ό μ¬μ©λλ€.
κ·Έλ μ§λ§ μ¬μ©ν  λλ§λ€ Connectionμ μμ±ν΄μ€μΌ νκ³ , μ€λ³΅λλ μ½λκ° λ§μ μ€μ  κ°λ°μλ μ μμ°μ΄λ λλμ΄λ€.

μ΄ JDBCλ₯Ό μ¬μ©νκΈ° μ½κ² λ§λ€μ΄μ£Όλ κ²μ΄ **Mybatis**μ΄λ€.
μκΉ λ§νλ―, SQL Mapperμ ν΄λΉνλ€. JDBCλ‘ μ²λ¦¬νλ λΆλΆμ μΌλΆλ₯Ό μ½λμ νλΌλ―Έν° μ€μ μΌλ‘ λ§€νμ λμ  ν΄μ€λ€.

```null
μ₯μ 
+ νμ΅μ΄ μ½λ€.
+ μμ€μ½λμ sqlμ λΆλ¦¬ν  μ μλ€.

λ¨μ 
+ λ°λ³΅μ μΈ μμμ΄ λ°λ³΅λλ€.
```



#### @JPA (Java Persistent API)

Java ORM κΈ°μ μ λν API νμ€ λͺμΈλ‘, μ΄κ² λν Javaμμ μ κ³΅νλ APIμ΄λ€.
μ¬μ©ν  λ JPA, Spring Data JPA, Hibernateλ₯Ό νΌλνκΈ° μ½λ€.

- JPAλ μλ° μ΄νλ¦¬μΌμ΄μμμ RDBMSλ₯Ό μ¬μ©νλ λ°©μμ μ μν μΈν°νμ΄μ€μ΄λ€.
  **λΌμ΄λΈλ¬λ¦¬κ° μλ**! -> κ΅¬νμ΄ μλ€.
- Spring Data JPAλ JPAλ₯Ό μ°κΈ° μ’κ² λ§λ€μ΄λμ λͺ¨λμ΄λ€.
  JPA interfaceλ₯Ό κ΅¬νν΄ **Repository**λΌλ μΈν°νμ΄μ€λ₯Ό μ κ³΅νλ€.
- Hibernateλ JPAμ κ΅¬νμ²΄μ΄λ€.

```null
μ₯μ 
+ CRUD μΏΌλ¦¬λ₯Ό μλμΌλ‘ μμ±ν΄μ€λ€.
+ Entityμ μμ±λ§ μΆκ°ν΄μ€λ€λ©΄ μΏΌλ¦¬λ₯Ό κ±΄λ€ νμκ° μλ€.

λ¨μ 
+ μλμ μΌλ‘ νμ΅μ΄ μ΄λ ΅λ€.
+ λ³΅μ‘ν μΏΌλ¦¬ μμ±μ΄ μ΄λ ΅λ€κ³  νλ€.
```



[μΆμ²] https://velog.io/@leeinae/Spring-Mybatis-JPA-Hibernate-%EB%B9%84%EA%B5%90



#### π‘ Spring Bean μ£Όμ λ°©λ²

#### 1. μ»΄ν¬λνΈ μ€μΊμ μ΄μ©ν λ±λ‘λ°©λ²

>  μ»΄ν¬λνΈ μ€μΊκ³Ό μλ μμ‘΄κ΄κ³ μ€μ 
>
> μ»΄ν¬λνΈ μ€μΊμ μλ¦¬λ κΈ°λ³Έμ μΌλ‘ @Component μ΄λΈνμ΄μμ΄ μμΌλ©΄ μλμΌλ‘ μ€νλ§ λΉμΌλ‘ λ±λ‘λλ€.
>
> >  μ°Έκ³ λ‘, @Component μ΄λΈνμ΄μμ @Controller , @Service, @Repositoryλ₯Ό ν¬ν¨νλ€.

- μ»΄ν¬λνΈ μ€μΊμ μ΄μ©ν λ°©λ²μ μ£Όλ‘ μ€λ¬΄μμ μ ννλ μ»¨νΈλ‘€λ¬, μλΉμ€, λ¦¬ν¬μ§ν λ¦¬ κ°μ κ³³μ μ¬μ©νλ€.
- **μ¦, κ³ μ ν λμ΄ λ°λμΌμ΄ μμ κ²½μ°! μ¬μ©νλ€κ³  λ³΄λ©΄ λλ€. λ¬΄μμ  μ°λκ±°λ³΄λ€ μν©μ λ§κ² μ¬μ©νλκ²μ΄ μ€μ!!**



#### 2. μλ°λ₯Ό ν΅ν μ§μ  λ±λ‘λ°©λ²

> **μλ° μ½λλ‘ μ§μ  λ±λ‘ν λλ Controllerλ μ»¨ν¬λνΈ μ€μΊμΌλ‘ μ¬λΌκ°κΈ° λλ¬Έμ @Controllerλ₯Ό μΆκ°ν΄μΌ νλ€.**

μ£Όλ‘ μ νν λμ§ μκ±°λ μν©μ λ°λΌ κ΅¬ν ν΄λμ€λ₯Ό λ³κ²½ν΄μΌ ν μΌμ΄ μκΈ°κ² λκ±°λ, κ·Έλ΄ μ¬μ§κ° μλ κ²½μ° μ§μ  μ€μ μ ν΅ν΄ λ±λ‘νλ€.

**μ¦, λ³κ²½λ  μΌ νΉμ μ¬μ§κ° μλ κ²½μ°μ μ§μ  λ±λ‘νκ²λλ©΄, μ½λλ₯Ό ν¬κ² μμ νμ§μμλ μ½κ² λ³κ²½ν  μ μλ μ₯μ μ΄ μλ€!!**

- λ³λμ Config νμΌμ μμ±νμ¬ μ§μ  μ£Όμνλ λ°©λ²μ΄λ€.

- μ€νλ§μ΄ μμλ λ @Configurationμ μ°Ύμκ°κ² λλ€.

  

#### π‘ Web Serverκ³Ό WASμ μ°¨μ΄μ 

### Web Server

1. **Web Serverμ κ°λ**
   - μννΈμ¨μ΄μ νλμ¨μ΄λ‘ κ΅¬λΆλλ€.
     1) νλμ¨μ΄
   - Web μλ²κ° μ€μΉλμ΄ μλ μ»΄ν¨ν°
     2) μννΈμ¨μ΄
     μΉ λΈλΌμ°μ  ν΄λΌμ΄μΈνΈλ‘λΆν° HTTP μμ²­μ λ°μ μ μ μΈ μ»¨νμΈ (.html .jpeg .css λ±)λ₯Ό μ κ³΅νλ μ»΄ν¨ν° νλ‘κ·Έλ¨
2. **Web Serverμ κΈ°λ₯**
   - HTTP νλ‘ν μ½μ κΈ°λ°μΌλ‘ νμ¬ ν΄λΌμ΄μΈνΈ(μΉ λΈλΌμ°μ  λλ μΉ ν¬λ‘€λ¬)μ μμ²­μ μλΉμ€ νλ κΈ°λ₯μ λ΄λΉνλ€.
     μμ²­μ λ°λΌ μλμ λ κ°μ§ κΈ°λ₯ μ€ μ μ νκ² μ ννμ¬ μννλ€.
     - κΈ°λ₯ 1)
       μ μ μΈ μ»¨νμΈ  μ κ³΅
       WASλ₯Ό κ±°μΉμ§ μκ³  λ°λ‘ μμμ μ κ³΅νλ€.
     - κΈ°λ₯ 2)
       λμ μΈ μ»¨νμΈ  μ κ³΅μ μν μμ²­ μ λ¬
       ν΄λΌμ΄μΈνΈμ μμ²­(Request)μ WASμ λ³΄λ΄κ³ , WASκ° μ²λ¦¬ν κ²°κ³Όλ₯Ό ν΄λΌμ΄μΈνΈμκ² μ λ¬(μλ΅, Response)νλ€.
       ν΄λΌμ΄μΈνΈλ μΌλ°μ μΌλ‘ μΉ λΈλΌμ°μ λ₯Ό μλ―Ένλ€.
3. **Web Serverμ μ**
   Ex) Apache Server, Nginx, IIS(Windows μ μ© Web μλ²) λ±



### WAS(Web Application Server)

1. **WASμ κ°λ**

   - DB μ‘°νλ λ€μν λ‘μ§ μ²λ¦¬λ₯Ό μκ΅¬νλ λμ μΈ μ»¨νμΈ λ₯Ό μ κ³΅νκΈ° μν΄ λ§λ€μ΄μ§ Application Server
   - HTTPλ₯Ό ν΅ν΄ μ»΄ν¨ν°λ μ₯μΉμ μ νλ¦¬μΌμ΄μμ μνν΄μ£Όλ λ―Έλ€μ¨μ΄(μννΈμ¨μ΄ μμ§)μ΄λ€.
   - βμΉ μ»¨νμ΄λ(Web Container)β νΉμ βμλΈλ¦Ώ μ»¨νμ΄λ(Servlet Container)βλΌκ³ λ λΆλ¦°λ€.
     - Containerλ JSP, Servletμ μ€νμν¬ μ μλ μννΈμ¨μ΄λ₯Ό λ§νλ€.
       μ¦, WASλ JSP, Servlet κ΅¬λ νκ²½μ μ κ³΅νλ€.

2. **WASμ μ­ν **

   - WAS = Web Server + Web Container
   - Web Server κΈ°λ₯λ€μ κ΅¬μ‘°μ μΌλ‘ λΆλ¦¬νμ¬ μ²λ¦¬νκ³ μνλ λͺ©μ μΌλ‘ μ μλμλ€.
     - λΆμ° νΈλμ­μ, λ³΄μ, λ©μμ§, μ°λ λ μ²λ¦¬ λ±μ κΈ°λ₯μ μ²λ¦¬νλ λΆμ° νκ²½μμ μ¬μ©λλ€.
       μ£Όλ‘ DB μλ²μ κ°μ΄ μνλλ€.

3. **WASμ μ£Όμ κΈ°λ₯**

   - νλ‘κ·Έλ¨ μ€ν νκ²½κ³Ό DB μ μ κΈ°λ₯ μ κ³΅
   - μ¬λ¬ κ°μ νΈλμ­μ(λΌλ¦¬μ μΈ μμ λ¨μ) κ΄λ¦¬ κΈ°λ₯
   - μλ¬΄λ₯Ό μ²λ¦¬νλ λΉμ¦λμ€ λ‘μ§ μν

4. **WASμ μ**
   Ex) Tomcat, JBoss, Jeus, Web Sphere λ±

   



#### μ¦, μμ μ΄μ©μ ν¨μ¨μ± λ° μ₯μ  κ·Ήλ³΅, λ°°ν¬ λ° μ μ§λ³΄μμ νΈμμ± μ μν΄ Web Serverμ WASλ₯Ό λΆλ¦¬νλ€. Web Serverλ₯Ό WAS μμ λκ³  νμν WASλ€μ Web Serverμ νλ¬κ·ΈμΈ ννλ‘ μ€μ νλ©΄ λμ± ν¨μ¨μ μΈ λΆμ° μ²λ¦¬κ° κ°λ₯νλ€.
[μΆμ²] https://gmlwjd9405.github.io/2018/10/27/webserver-vs-was.html



#### π‘ JARκ³Ό WARμ μ°¨μ΄μ 

> **JAR** (**J**ava **Ar**chive), **WAR** (**W**eb **A**pplication A**r**chive) λͺ¨λ JAVAμ jar ν΄μ μ΄μ©νμ¬ μμ±λ μμΆ(μμΉ΄μ΄λΈ) νμΌμ΄λ©° **μ΄νλ¦¬μΌμ΄μμ μ½κ² λ°°ν¬νκ³  λμμν¬ μ μλλ‘ μλλ‘ κ΄λ ¨ νμΌ(λ¦¬μμ€, μμ±νμΌ λ±)λ€μ ν¨ν€μ§**ν΄μ£Όλ κ²μ΄ μ£Ό μ­ν 

#### **JAR & WAR**

- **java κΈ°λ°μ applicationμ λ°°ν¬ ννμ΄λ€.**
- **JAVA JAR TOOLμ μ΄μ©νμ¬ μμΆν μμΆ νμΌμ΄λ€. ( μ¦, λμ΄ κ°μ μμΆ νν )**
- **JARμ WARλ μ¬μ© λͺ©μ μ΄ λ€λ₯΄λ€.**



<img src="image/jar_war.png" style="zoom:33%;" />

#### **JAR**

- Java ARchive
- path μ λ³΄λ₯Ό μ μ§ν μνλ‘ μμΆνλ€.
- μλ° ν΄λμ€ νμΌκ³Ό, κ° ν΄λμ€λ€μ΄ μ¬μ©νλ κ΄λ ¨ λ¦¬μμ€νμΌ λ° λ©νλ°μ΄ν°μ μμΆν νμΌμ΄λ€.
- μ€μ λ‘λ ZIP νμΌ ν¬λ§·μΌλ‘ μμΆλ νμΌμ΄λ€.

#### **WAR**

- Web application ARchive
- μΉ μ΄νλ¦¬μΌμ΄μμ μ΄λ»κ² μ€μ ν  μ§μ λν μ μκ° μλ web.xml νμΌμ΄ μλ€.
- μλ° μλ² νμ΄μ§, μλ° μλΈλ¦Ώ, μλ° ν΄λμ€, XML, νμΌ, νκ·Έ λΌμ΄λΈλ¬λ¦¬, μ μ  μΉνμ΄μ§(HTML κ΄λ ¨ νμΌ) λ° μΉ applicationμ κ΅¬μ±ν  λ νμν μμμ μμΆν jar νμΌμ΄λ€.

