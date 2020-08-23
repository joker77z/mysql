# 0822 CREATE, READ
- setup mysql

- how to use mysql?  
1. cd C:\Program Files\MySQL\MySQL Server 8.0\bin  
2. mysql -uroot -p > password input  
3. CREATE DATABSE DATABASE_NAME;  
4. SHOW DATABASES;  
5. CREATE TABLE TABLE_NAME ( --- );  
6. SHOW TABLES;  
7. DESC(or DESCRIBE) TABLE_NAME;  

- how to insert data in table?
1. INSERT INTO(---) VALUES('---')

- how to show data in table?
1. SELECT * FROM TABLE_NAME;

- can limit on select
1. SELECT * FROM TABLE_NAME LIMIT 2;

- can order by select
1. SELECT * FROM TABLE_NAME ORDER BY column_name ASC|DESC;

# 0822 UPDATE, DELETE
easy.

# 0823 TABLE Distribute, Join
1. 기존 TABLE을 RENAME한다. ex) topic → topic_BACKUP  
2. create topic table  
3. create author table  
4. insert into data to table  

5. SELECT topic.id, title .... FROM topic LEFT JOIN author ON topic.author_id = author.id;
// 이렇게 하면 하나로 합쳐진 테이블을 볼 수 있고 만약에 author에서 데이터를 하나 수정하게 되면 모든 테이블에 연동되어 있는 id값이 있기 때문에 반영이 한번에 된다.
// 변경할 때는 UPDATE 테이블이름 SET profile = 'database administrator' WHERE id = 2; // 이런식으로 id 2번의 profile컬럼의 값을 database administrator로 변경하면 된다.

- how to use mySQL workbench  
1. new schema  
2. new table  
3. insert table data  
