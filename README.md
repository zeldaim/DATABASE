 DATABASCREATE TABLE
DEPT(
DEPT_ID INTEGER NOT NULL AUTO_INCREMENT
, DEPT_NM VARCHAR(20)
, DEPT_CNT INTEGER
, DEPT_MGR_NO INTEGER
, CRT_DEPT DATETIME
, PRIMARY KEY(DEPT_ID)
);


create table BTC
(ID VARCHAR(10)
,NAME VARCHAR(20)
,ADDR VARCHAR(50)
,PHONE_NUM INTEGER 
,CLASS VARCHAR(5)
);

create table BTC_1_1 
(ID VARCHAR (10) primary key 
,NAME VARCHAR(20)
,ADDR VARCHAR(50) 
,PHONWE_NUM INTEGER
,CLASS VARCHAR(5)
);

create table BTC_2
(ID VARCHAR(10) 
,NAME VARCHAR(20)
,ADDR VARCHAR(50)
,PHONE_NUM INTEGER 
,CLASS VARCHAR(5)
,PRIMARY key (ID)
,unique KEY(PHONE_NUM)
);

create TABLE BTC_3
(ID VARCHAR(10)
,NAME VARCHAR(20)
,ADDR VARCHAR(50) not null 
,PHONE_NUM INTEGER 
,CLASS VARCHAR(5) check (CLASS in ('BTC_1', 'BTC_2'))
,primary key (ID) 
,unique key(PHONE_NUM)
);

create table member 
(MEM_ID CHAR(8) not null primary key
,MEM_NAME VARCHAR(10) not null 
,MEM_NUMBER INTEGER not null  
,ADDR CHAR(2) not null 
,PHONE1 CHAR(3)  
,PHONE2 CHAR(13) 
,HEIGHT smallint
,DEBUT_DATE DATE); 

```
insert into member values('01','이현정',2323,'경기','010','1234234',23,'2001-01-01'); 
```
```
create table departments_1 
(dept_no char(4) not null
,dept_name varchar(40) not null 
,primary key(dept_no)
,unique key(dept_name)
);

```