🔄 Previous Session Recap (Session–01)

Data = Information about a real-world object.
Database = Collection of related data.
DBMS = Software used to store and manage data.
Traditional systems used books and registers.
File systems suffered from redundancy and inconsistency.
Database software provides security, integrity, and fast retrieval.
Database software is classified into:

RDBMS
NRDBMS (NoSQL)

📖 Current Session Topics
Types of Database Software
Introduction to SQL
Features of SQL
SQL Query Examples
Introduction to Oracle

1️⃣ TYPES OF DATABASE SOFTWARE

Database software is used to store and manage application data.

Real-Time Examples

Internet Banking
Amazon
Flipkart
College Management Systems

All application data is stored inside databases.

🔵 RDBMS (Relational Database Management System)

Examples
Oracle
MySQL
SQL Server
PostgreSQL
DB2

Features
Data Stored in Tables
Customer_Id	Customer_Name	Location
101	        Mahesh	      Hyderabad

RDBMS stores data in tables.

Important Terminology

Database Term	Meaning
Table	Relation

Column	Field / Attribute

Row	Tuple / Record

Structured Format

Data follows a predefined structure.

Example:

RollNo	Name	Branch
101	    Mahesh	CSE

Real-Time Usage

Banking Applications
Railway Reservation Systems
E-Commerce Websites
ERP Applications

Most enterprise applications use RDBMS databases.

🟢 NoSQL / NRDBMS
Examples
MongoDB
Cassandra
Redis
HBase
DynamoDB
Data Storage Formats
Document-Based
{
  "id":101,
  "name":"Mahesh"
}

Key-Value Based
101 → Mahesh
Column-Based

Stores data column-wise.

Graph-Based

Stores relationships between data.

2️⃣ INTRODUCTION TO SQL
What is SQL?
SQL = Structured Query Language

SQL is used to communicate with RDBMS databases.

Definition

SQL is a database language used to store, retrieve, update, and manage data.

3️⃣ FEATURES OF SQL
SQL is a Query Language

Used to write queries and communicate with databases.

Example:

SELECT * FROM customers;
SQL is Easy to Read

SQL statements resemble English sentences.

Example:

SELECT * FROM customers;

Meaning:

Select all records from customers table.

SQL is Case Insensitive

Both statements are valid:

SELECT * FROM customers;
select * from customers;

ANSI Standard Language

SQL is standardized by ANSI.

Therefore the same SQL concepts work in:

Oracle
MySQL
PostgreSQL
SQL Server
Semicolon is Mandatory

Every SQL statement ends with:

;

Example:

SELECT * FROM customers;
One Statement Executes at a Time

SQL executes one query at a time.

For multiple statements and business logic, we use:

PLSQL

Procedural Language using SQL.

4️⃣ SQL QUERY EXAMPLES
Customer Table
Customer_Id	Customer_Name	Customer_Location
1025	        Mahesh	    Hyderabad
1026	        Suresh	    Delhi
1027	        Rajesh	    Bangalore
1028	        Nagesh	    Chennai
1029	        Naresh	    Pondicherry

Example 1: Customers from Hyderabad
SELECT *
FROM customers
WHERE customer_location='Hyderabad';

Output

Customer_Id	Customer_Name	Customer_Location
1025	      Mahesh	      Hyderabad

Example 2: Retrieve All Customers
SELECT *
FROM customers;

Returns all rows from the table.

Example 3: Find Customer ID by Name

SELECT customer_id
FROM customers
WHERE customer_name='Mahesh';

Output
Customer_Id
1025

5️⃣ INTRODUCTION TO ORACLE
About Oracle

Oracle is one of the most popular relational database management systems.

Developed by the company Oracle Corporation.

Why Oracle?
Advantages
High Performance
Strong Security
Large Storage Capacity
Reliability
Multi-User Support
Enterprise-Level Features
Used By
Banks
Airlines
Telecom Companies
E-Commerce Companies
Large Enterprises

🎯 Session–02 Summary
RDBMS stores data in tables.
NoSQL stores data in multiple formats.
SQL stands for Structured Query Language.
SQL is used to communicate with databases.
SQL is case-insensitive.
Every SQL statement ends with a semicolon (;).
Oracle is a popular RDBMS database software.
PLSQL is used when multiple SQL statements are required.
