# day2
## * 스키마의 사용
### - 데이터베이스 생성 : CREATE DATABASE DB명;
### - 데이터베이스 삭제 : DROP DATABASE DB명;
### - 데이터베이스 확인 : SHOW DATABASES;
### - 데이터베이스 선택 : USE DB명;
![image](https://user-images.githubusercontent.com/89372116/137950779-c174dc47-be7f-447d-94ad-0868ff2e2722.png)
## * SQL이란?
### -  데이터베이스를 사용할 때, 데이터베이스에 접근할 수 있는 데이터베이스 하부 언어
## * 테이블(표)의 구조
![image](https://user-images.githubusercontent.com/89372116/137949063-380800ee-683f-443b-8950-0ddc4755926c.png)
## * 테이블의 생성
### - 테이블 생성
```
CREATE TABLE 테이블명(
  칼럼명1 데이터타입(길이),
  칼럼명2 데이터타입(길이),
          .
          .
          .
 PRIMARY KEY(칼럼명)
 );
 ```
### - 사용할 데이터타입
#### -> INT(m) : 정수형
#### -> VARCHAR(size) : 가변형 문자열
#### -> TEXT(size) : 65,535자까지 가능한 문자열
#### -> DATETIME : 날짜와 시간
![image](https://user-images.githubusercontent.com/89372116/137954910-bbc9f24d-e7a4-4e7e-839b-b32dcb20ea8c.png)
 
