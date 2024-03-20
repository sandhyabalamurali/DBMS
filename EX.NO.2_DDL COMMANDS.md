# EXP NO 2: DATA DEFINITION LANGUGE COMMANDS 
### DATE
## AIM:
To create a student database and execute DDL queries using SQL.


## THEORY
### DDL (Data Definition Language)

* DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database schema.
* It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database.
* DDL is a set of SQL commands used to create, modify, and delete database structures but not data.
* These commands are normally not used by a general user, who should be accessing the database via an application.

 
### List of DDL commands: 
1. CREATE: This command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers).
2. DROP: This command is used to delete objects from the database.
3. ALTER: This is used to alter the structure of the database.
4. TRUNCATE: This is used to remove all records from a table, including all spaces allocated for the records are removed.
5. RENAME: This is used to rename an object existing in the database.

## Query:
### 1) Create a database studentdb
### SQL QUERY:
```
create database studentdbb;
```

### OUTPUT:
![281072399-58fc5109-3fe3-4b71-adfa-c8de97a3eb0c](https://github.com/sandhyabalamurali/DBMS/assets/115525118/fdae06ef-b168-48d4-acd0-01046d1e3b52)
![281073166-a4e4ad5f-3b5d-4d4c-b347-54957dca3420](https://github.com/sandhyabalamurali/DBMS/assets/115525118/e6f94b61-bfb1-4aca-944a-a79583b3e931)

### 2) Create a table student  and insert any two rows with the following fieds RegisterNumber,Name,Age,Address,Phone number

### SQL QUERY: 
```
 create table student(RegisterNumber int,Name varchar(100),Age int,Address varchar(250),PhoneNumber int) ;
```

### OUTPUT:
![image](https://github.com/sandhyabalamurali/DBMS/assets/115525118/11896e64-0a36-4c35-8546-77bd8d1432f3)

### 3) Alter the above student table by adding another attribute department
### SQL QUERY: 
```
 alter table student add dept varchar(20);
```
### OUTPUT:
![image](https://github.com/sandhyabalamurali/DBMS/assets/115525118/53c59fbf-3c45-4d07-ab75-6012be6388e1)

### 4) Rename the student table to mystudent

### SQL QUERY: 
```
alter table student rename to mystudent;
```


### OUTPUT:
![image](https://github.com/sandhyabalamurali/DBMS/assets/115525118/b28f9097-f38f-43ce-b7c3-dbe66500f290)

### 5) Delete the mystudent rows using truncate keyword

### SQL QUERY: 
```
 truncate table mystudent;
```

### OUTPUT:
![image](https://github.com/sandhyabalamurali/DBMS/assets/115525118/43c30f03-3004-423c-bc0b-d7f4893d2cac)

### 4) Drop the mystudent table
 
### SQL QUERY: 
```
 drop table mystudent;
```

### OUTPUT:

![image](https://github.com/sandhyabalamurali/DBMS/assets/115525118/c45d03e8-c3b1-4885-bdf6-92d54900b3f6)

## Result:
         Thus the basic DDL commands in SQL are executed. 


