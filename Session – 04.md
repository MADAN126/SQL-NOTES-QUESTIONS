🔄 Previous Session Recap (Session–03)
SQL Commands are also called SQL Statements or Queries.
Every SQL statement must end with a semicolon (;).
SQL Commands are classified into 5 categories:
DDL (Create, Alter, Drop, Truncate)
DML (Insert, Update, Delete)
DCL (Grant, Revoke)
DRL (Select)
TCL (Commit, Rollback, Savepoint)
Database Objects include:
Tables
Views
Sequences
Indexes
Stored Procedures
Stored Functions

📖 Current Session Topics
Introduction to Database Tables
Creating a Table using CREATE
Naming Conventions in Oracle
Inserting Data using INSERT
Retrieving Data using SELECT
Complete Customer Table Example

1️⃣ Introduction to Database Tables

What is a Table?

A Table is a database object used to store data in the form of rows and columns.

Example: Customer Table
Customer_ID	Customer_Name	Gender	Age	Location
101	        Mahesh	      Male	  35	Hyderabad
102	        Ashok	        Male	  35	Hyderabad

Real-Life Flow
Create Table
      ↓
Insert Data
      ↓
Retrieve Data

Commands Used
Task Command   Type    	Command
Create Table	  DDL	    CREATE
Insert Data	    DML	    INSERT
Retrieve Data	  DRL	    SELECT
2️⃣ Creating a Table using CREATE
CREATE Command

The CREATE command is used to create database objects.

Syntax
CREATE TABLE table_name(
    column1 datatype,
    column2 datatype,
    column3 datatype
);
Example: Customer Table

Requirements:

Field	Data Type
Customer ID	Number
Customer Name	String
Gender	String
Age	Number
Location	String
Query
CREATE TABLE ashokit_customers(
    customer_id NUMBER,
    customer_name VARCHAR(50),
    gender VARCHAR(15),
    age NUMBER,
    location VARCHAR(50)
);
Output
Table Created.
3️⃣ Naming Conventions in Oracle

Whenever naming a:

Table
Column
View
Sequence
Index

follow these rules.

Rule 1

Name must start with an alphabet.

Valid
customer
employee
student1
Invalid
1customer
@employee

Rule 2

Allowed Characters

a-z
A-Z
0-9
@
$
#
_

Example:

customer_1
emp$details
student#data

Rule 3

Names are Case Insensitive

CUSTOMERS
customers
Customers

All are treated as the same name.

Rule 4

Reserved Keywords Not Allowed

Invalid
CREATE TABLE SELECT(...)

SELECT is a keyword.

Rule 5

Spaces Are Not Allowed

Invalid
customer table
employee details
Valid
customer_table
employee_details

4️⃣ Inserting Data using INSERT
INSERT Command

Used to add records into a table.

INSERT belongs to

DML (Data Manipulation Language)
Method 1: Specify Column Names

Syntax
INSERT INTO table_name
(column1,column2,column3)
VALUES(value1,value2,value3);

Example
INSERT INTO ashokit_customers
(customer_id,customer_name,gender,age,location)
VALUES
(1,'Mahesh','Male',35,'Hyderabad');
INSERT INTO ashokit_customers
(customer_id,customer_name,gender,age,location)
VALUES
(2,'Ashok','Male',35,'Hyderabad');

Method 2: Insert Without Column Names

Syntax
INSERT INTO table_name
VALUES(value1,value2,value3);
Example
INSERT INTO ashokit_customers
VALUES(3,'Rajesh','Male',40,'Mumbai');
Note

Values must follow the exact column order.

Method 3: Runtime Input
Syntax
INSERT INTO ashokit_customers
VALUES(&customerId,
       &customerName,
       &gender,
       &age,
       &location);

Oracle asks for values during execution.

5️⃣ Retrieving Data using SELECT
SELECT Command

Used to retrieve data from a table.

SELECT belongs to
DRL (Data Retrieval Language)
Syntax
SELECT * FROM table_name;
Meaning
Symbol	Meaning
*	All Columns
Example
SELECT * FROM ashokit_customers;

Output

Customer_ID	Customer_Name	Gender	Age	Location
1          	Mahesh	Male	35	Hyderabad
2	          Ashok	  Male	35	Hyderabad
3	          Rajesh	Male	40	Mumbai
6️⃣ Complete Flow Example
Step 1 – Create Table
CREATE TABLE ashokit_customers(
    customer_id NUMBER,
    customer_name VARCHAR(50),
    gender VARCHAR(15),
    age NUMBER,
    location VARCHAR(50)
);

⬇

Step 2 – Insert Records
INSERT INTO ashokit_customers
VALUES(1,'Mahesh','Male',35,'Hyderabad');

⬇

Step 3 – Retrieve Records
SELECT * FROM ashokit_customers;

⬇

Result

Customer data displayed successfully.

💡 Useful SQL*Plus Command

To avoid line wrapping:

SET LINESIZE 300;

This increases output width in SQL*Plus.

🎯 Session Summary
Table is a database object used to store data.
CREATE command is used to create tables.
INSERT command is used to add records.
SELECT command is used to retrieve records.
Oracle naming conventions must be followed.
A typical database operation follows:
CREATE
   ↓
INSERT
   ↓
SELECT

❓ Interview Questions

Q1. What is a Table?

A database object that stores data in rows and columns.

Q2. Which command is used to create a table?

CREATE

Q3. Which command is used to insert records?

INSERT

Q4. Which command is used to retrieve records?

SELECT

Q5. What does * mean in SELECT *?

It represents all columns.

Q6. Can a table name start with a number?

No.

Q7. Which command category does CREATE belong to?

DDL (Data Definition Language).

⚡ Quick Revision Sheet
Command	Category	Purpose
CREATE	DDL	Create Object
INSERT	DML	Insert Data
SELECT	DRL	Retrieve Data
Golden Memory Rule
Table Creation
      ↓
Data Insertion
      ↓
Data Validation

CREATE → INSERT → SELECT 🚀
