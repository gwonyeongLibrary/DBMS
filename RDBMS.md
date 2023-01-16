# SQL의 이해(Structures Query Langauage)

- 데이터베이스에 있는 필요한 정보를 사용할 수 있도록 도와주는 언어
- 사용방법이나 문법이 다른 언어(Java, C, C#등)보다 단순하다.
- 하나를 배워두면 모든 DBMS에서 사용 가능하다.
- 인터프리터 : 언어를 입력받으면 그 때 분석해서 사용
- `대소문자를 구분하지 않음`

# DML(Data Manipulation Langauage)

- 테이블의 데이터를 조작하는 기능
- 테이블의 레코드를 CRUD

| SQL    | DESC                                      |
| ------ | ----------------------------------------- |
| INSERT | 데이터베이스 객체에 데이터를 입력한다.    |
| DELETE | 데이터베이스 객체에 데이터를 삭제한다.    |
| UPDATE | 데이터베이스 객체 안의 데이터를 수정한다. |
| SELECT | 데이터베이스 객체 안의 데이터를 조회한다. |

[DML](https://www.notion.so/DML-ba989e54129b4799ba01cccff5c4e083)

[DML 2](https://www.notion.so/DML-2-ecc1b29db5b640739982475e69460025)

[DML 3](https://www.notion.so/DML-3-6550bee0eeb8483d906ff6f3fe8db26d)

[DML4 (JOIN)](https://www.notion.so/DML4-JOIN-1a33c18ded2b42d5a5cc210cad196e74)

[DML](https://www.notion.so/DML-1a67221a909941d591ed0a4c15be4a8f)

[DML](https://www.notion.so/DML-0ddf83b275f04c34bb774bfd2d3bfc4a)

---

# DDL(Data Definition Langauage)

- DB, 테이블의 스키마를 정의, 수정하는 기능
- 테이블 생성, 컬럼 추가, 타입 변경, 각종 제약조건 지정, 수정 등

| SQL    | DESC                                              |
| ------ | ------------------------------------------------- |
| CREATE | 데이터베이스 객체를 생성한다.                     |
| DROP   | 데이터베이스 객체를 삭제한다,                     |
| ALTER  | 기존에 존재하는 데이터베이스 객체를 다시 정의한다 |

---

# DCL(Data Control Language)

- DB나 테이블의 접근권한이나 CRUD 권한을 정의하는 기능
- 특정 사용자에게 테이블의 조회권한 허가, 금지 등

| SQL    | DESC                                           |
| ------ | ---------------------------------------------- |
| GRANT  | 데이터베이스 객체에 권한을 부여 한다.          |
| REVOKE | 이미 부여된 데이터베이스 객체 권한을 취소한다. |
