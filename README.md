## EXP NO 1: DATA DEFINITION LANGUGE COMMANDS IN RDBMS
### AIM:
To create a student database and execute DDL queries using SQL.

### DDL (Data Definition Language)
DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database schema. It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database. DDL is a set of SQL commands used to create, modify, and delete database structures but not data. These commands are normally not used by a general user, who should be accessing the database via an application.
### List of DDL commands:
CREATE: This command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers). DROP: This command is used to delete objects from the database. ALTER: This is used to alter the structure of the database. TRUNCATE: This is used to remove all records from a table, including all spaces allocated for the records are removed. RENAME: This is used to rename an object existing in the database.
### Query:
#### 1) Create a table student with the following fieds rollno,name,age,address,phoneno.
##### SQL QUERY:
```
create table studenttable(rollnumber int,studentname char(20),age int,address char(20),phonenumber int);
insert into studenttable values ('22009033','Yuvarani','19','Thandalam','6383257388');
insert into studenttable values ('22009666','Panimalar','19','Vellore','8825733681');
insert into studenttable values ('22006962','Menarossini','20','Thoothukudi','9894236651');
insert into studenttable values ('22009006','Keerthana','18','Arakonam','7200357537');
insert into studenttable values ('22008449','Jayashree','19','Avadi','9445295666');
select * from studenttable;
```
##### OUTPUT:
![Screenshot 2023-09-14 182938](https://github.com/Yuvaranithulasingam/F2_DBMS/assets/121418522/6cb91567-e255-4bb1-b4b7-86569f3fb534)

#### 2) Change the above student table by adding another attribute department
##### SQL QUERY:
```
alter table studenttable add department char(20);
update studenttable set department='CSE(IOT)' where rollnumber=22009033;
update studenttable set department='CSE(CyberSecurity)' where rollnumber=22009666;
update studenttable set department='CSE' where rollnumber=22006962;
update studenttable set department='AI' where rollnumber=22009006;
update studenttable set department='ECE' where rollnumber=22008449;
select * from studenttable;
```
##### OUTPUT:
![Screenshot 2023-09-14 183533](https://github.com/Yuvaranithulasingam/F2_DBMS/assets/121418522/52669bdc-ff57-4935-a255-7b8e6e15a4f9)

#### 3) Drop the student table
##### SQL QUERY:
```
DROP TABLE studenttable;
```
##### OUTPUT:
![Screenshot 2023-09-14 192248](https://github.com/Yuvaranithulasingam/F2_DBMS/assets/121418522/2f804b25-13c2-4c68-844f-80c41d02a1b8)

#### 4) Delete the student table using truncate keyword
##### SQL QUERY:

##### OUTPUT:
#### 5) Rename the student table to mystudent
##### SQL QUERY:
##### OUTPUT:
