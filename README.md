# EXP NO 1: DATA DEFINITION LANGUGE COMMANDS IN RDBMS

## AIM:
To create a student database and execute DDL queries using SQL.


## DDL (Data Definition Language)
<div align="justify">
DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database schema. It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database. DDL is a set of SQL commands used to create, modify, and delete database structures but not data. These commands are normally not used by a general user, who should be accessing the database via an application.
</div>
 
## List of DDL commands: 
<div align="justify">
CREATE: This command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers).
DROP: This command is used to delete objects from the database.
ALTER: This is used to alter the structure of the database.
TRUNCATE: This is used to remove all records from a table, including all spaces allocated for the records are removed.
RENAME: This is used to rename an object existing in the database.
</div>

## Query:
### 1) Create a table student with the following fieds rollno,name,age,address,phoneno.

### SQL QUERY:
CREATE TABLE student (
  rollno INT NOT NULL,
  name VARCHAR(255) NOT NULL,
  age INT NOT NULL,
  address VARCHAR(255),
  phoneno VARCHAR(255)
); 


### OUTPUT:
![output](./images/o1.png)

### 2) Change the above student table by adding another attribute department

### SQL QUERY: 
ALTER TABLE student ADD department VARCHAR(255);

### OUTPUT:
![output](./images/o2.png)


### 3) Drop the student table
 
### SQL QUERY: 
DROP TABLE student;


### OUTPUT:
![output](./images/o3.png)


### 4) Delete the student table using truncate keyword

### SQL QUERY: 
TRUNCATE TABLE student;


### OUTPUT:
![output](./images/o4.png)



### 5) Rename the student table to mystudent1

### SQL QUERY: 
RENAME TABLE student TO mystudent1;


### OUTPUT:
![output](./images/o5.png)
