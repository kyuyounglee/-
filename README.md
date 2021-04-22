-- 사용자 추가(id : spring5 / psw : spring5)
create user 'spring5'@'localhost' identified by 'spring5';

-- 데이터베이스 추가
create database spring5fs character set=utf8;

-- 사용자에 대한 권한 추가
grant all privileges on spring5fs.* to 'spring5'@'localhost';

-- 데이블 생성
create table spring5fs.MEMBER(
ID INT auto_increment primary key,
EMAIL varchar(255),
PASSWORD varchar(100),
NAME varchar(100),
REGDATE datetime,
unique key(EMAIL)
)engine = InnoDB character set = utf8;


차주 수업마무리
1.전체 리뷰 - 복습
2.java->servlet->jsp->spring
3.스프링 부트
4.AOP
5.화면 ui -> javascript
6.css-> bootstrip
