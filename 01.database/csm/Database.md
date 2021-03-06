## Database

#### 💡 File (파일 시스템) vs DBMS (일반적인 RDBMS)

- 파일 시스템은 계층적 디렉터리 구조로 이루어져 있으며, 파일을 저장 장치에 저장합니다.
  파일 시스템은 데이터 불일치, 무결성 유지의 어려움 등의 단점이 있으며 이를 극복하고자 만들어진 것이 DBMS입니다.
  DBMS는 table 구조로 데이터를 저장하기 때문에 접근이 용이합니다. DBMS는 데이터 중복을 최소화하고, 무결성과 보안성 유지라는 특징이 있습니다.



##### File (파일 시스템)

- 파일 시스템 : 파일(데이터의 모임)을 저장 장치에 저장하고 사용하기 위한 일종의 규칙이나 체계
- 파일의 기본적인 구성 요소 : 순차적인 <u>레코드</u>(파일을 다룰 때 실제로 읽고 쓰는 단위로서 사용되는 데이터 단위)



###### 구조

- 계층적 디렉터리 구조



###### 특징

- 데이터 정의가 응용 프로그램에 내포되어 있다.
- 프로그램에서 데이터를 접근하고 조작하는 것 이외에 별도의 제어가 없다.

-> 많은 단점 발생



###### 단점

- 데이터 간 불일치가 발생할 수 있다.
- 다수 사용자를 위한 동시성 제어가 제공되지 않는다.
- 쉬운 질의어가 제공되지 않는다.
- 보안 기능이 미흡하다.
- 회복 기능이 없다.
- 데이터 독립성이 없어 유지보수 비용이 크다.
- 데이터 모델링 개념이 부족하다.
- 데이터 무결성을 유지하기가 어렵다.
- 생산성이 낮다.
- 데이터 공유가 잘 되지 않는다.



##### DBMS (RDBMS)

- 파일 시스템의 단점을 극복하고자 만들어짐 -> 단점을 역으로 생각하면 DBMS의 장점



###### 구조

- table 형태로 데이터를 저장한다.



##### 가장 큰 차이점

- 무결성의 원칙



#### 💡 Schema가 무엇인가요?

- 스키마는 데이터베이스의 구조와 관계, 제약 조건 등을 정의한 것입니다.



##### Schema (스키마)

- 데이터베이스를 구성하는 데이터 개체(Entity), 속성(Attribute), 관계(Relationship) 및 데이터 조작 시 데이터 값들이 갖는 제약 조건 등에 관해 전반적으로 정의한다.
- 스키마는 외부 스키마, 개념 스키마, 내부 스키마로 나눠진다.



###### 외부 스키마 = 사용자 뷰 (View)

- 사용자나 응용 프로그래머가 각 개인의 입장에서 필요로 하는 데이터베이스의 논리적 구조를 정의한 것



###### 개념 스키마 = 전체적인 뷰 (View)

- 데이터베이스의 전체적인 논리적 구조. 모든 응용 프로그램이나 사용자들이 필요로 하는 데이터를 종합한 조직 전체의 데이터베이스로 하나만 존재한다.
- 개체간의 관계와 제약 조건을 나타내고, 데이터베이스의 접근 권한, 보안 및 무결성 규칙에 관한 명세를 정의한다.



###### 내부 스키마 = 저장 스키마

- 물리적 저장장치의 입장에서 본 데이터베이스 구조
- 실제로 데이터베이스에 저장될 레코드의 물리적인 구조를 정의, 저장 데이터 항목의 표현방법, 내부 레코드의 물리적 순서 등을 나타낸다.
- 시스템 프로그래머나 시스템 설계자가 보는 관점의 스키마
