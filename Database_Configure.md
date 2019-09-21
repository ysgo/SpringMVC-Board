# [ Database Configure ]

## 테이블 생성

```sql
create table news (
    id varchar2(100) primary key,
    writer varchar2(100),
    title varchar2(100),
    content varchar2(4000),
    writedate date default sysdate,
    cnt number(38)
);
```

## 시퀀스 생성

```sql
# 데이터 생성시 자동으로 1씩 증가하는 news 시퀀스 생성
create sequence news_seq
start with 1
increment by 1;
```

## 테이블 조회 및 삭제

```sql
# 데이터베이스의 테이블 전체 조회
select * from tab;

# news 테이블 데이터 조회
select * from news;

# news 테이블 삭제
drop table news;
```

