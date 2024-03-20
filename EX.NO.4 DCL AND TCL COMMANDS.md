# EX.NO 4 Data Control Language (DCL) Commands and Transaction Control Languages (TCL) in SQL
### DATE:
## AIM:
To create a manager database and execute DML queries using SQL.

# THEORY
## Data Control Language (DCL) commands
* Data control language (DCL) is used to access the stored data.
* It is mainly used for revoke and to grant the user the required access to a database.
## List of DCL commands: 
1. GRANT : It is used to insert data into a table.
2. REVOKE: It is used to update existing data within a table.
## Transaction control language(TCL) commands
1. COMMIT : COMMIT command in SQL is used to save all the transaction-related changes permanently to the disk
2. START TRANSACTION : to start the transaction
3. ROLLBACK : undo the transaction upto savepoint 
4. SAVEPOINT : create a savepoint to save the different parts of the same transaction using different names

### Q1) Create a table employee with employee id ,name and Address

### QUERY:

```
create table employee(
emp_id numeric,
emp_name varchar(10),
addr varchar(40)
);
```
### OUTPUT:
![image](https://github.com/sandhyabalamurali/DBMS/assets/115525118/73ef9cfc-57d9-46a6-af6f-ccac87d34dd9)

### Q2) Insert three rows into emploee table 


### QUERY:

```
insert into employee values(1,'Luffy','EastBlue');
insert into employee values(2,'Shanks','GodValley');
insert into employee values(3,'Grap','MarinFord');
```
### OUTPUT:
![image](https://github.com/sandhyabalamurali/DBMS/assets/115525118/fb83c1d5-90f0-4e2b-b4c5-1bfb7ba2280f)

### Q3) Start the transaction and create a save point s1.

### QUERY:

```
exec savepoint A;
```
### OUTPUT:
![image](https://github.com/sandhyabalamurali/DBMS/assets/115525118/5c0fb79e-1d25-4b51-8272-374ea8a02586)

### Q4) Perform insertion into employee table.

### QUERY:

```
insert into employee values(4,'Robin','EniesLobby');
SELECT * FROM employee;
```
### OUTPUT:
![image](https://github.com/sandhyabalamurali/DBMS/assets/115525118/46e61ae7-ebbc-4e1a-be8f-17f6a26b6a60)


### Q6)	Display the employee table and create a save point s2 .


### QUERY:
```
select * from employee;
exec savepoint s2;
```

### OUTPUT:

![image](https://github.com/sandhyabalamurali/DBMS/assets/115525118/072f436e-82d2-42ea-9b37-08de15e68399)

### Q7)	Perform updation on any one of the row.


### QUERY:

```
update employee set emp_name='Nico Robin' where emp_id=4;
```
### OUTPUT:
![image](https://github.com/sandhyabalamurali/DBMS/assets/115525118/3159acc0-9971-42a7-975a-c9976eac920b)


### Q8) Display the employee table and rollback to  save point s2 


### QUERY:
```
SELECT * FROM employee;
ROLLBACK TO A;
```

### OUTPUT:
![image](https://github.com/sandhyabalamurali/DBMS/assets/115525118/23b2f215-91cb-4a5f-bb08-96cbc13d0404)


### Q9) Display the employee table and commit the changes; 


### QUERY:


### OUTPUT:


### Q10) Rollback to save point s1;


### QUERY:


### OUTPUT:


### Q11)	Create a new user and grant access to any one database with "insert and update"


### QUERY:


### OUTPUT:


### Q12) Check the user access and display the result 


### QUERY:


### OUTPUT:

### Q13) Revoke the privillages.

### QUERY:


### OUTPUT:


## RESULT :
Thus the basic TCL and DCL commands are executed.
