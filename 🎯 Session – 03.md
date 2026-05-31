🔄 Previous Session Recap (Session–02)
Learned about SQL (Structured Query Language).
SQL is used to communicate with RDBMS databases.
SQL is a case-insensitive language.
Every SQL statement ends with a semicolon (;).
Learned basic SQL queries using SELECT statements.
Understood the difference between RDBMS and NoSQL databases.
Introduction to Oracle Database and its importance.


6️⃣ Introduction to SQL Commands
What are SQL Commands?

SQL Commands are also called:

SQL Statements
SQL Queries
Definition

A SQL Command is a predefined statement used to perform a specific operation on a database.

Example
SELECT * FROM emp;

This retrieves all records from the EMP table.

Important Rule

Every SQL statement must end with:

;

Example:

SELECT * FROM emp;
7️⃣ Types of SQL Commands

SQL Commands are divided into five categories.

SQL Commands
     │
     ├── DDL
     ├── DML
     ├── DCL
     ├── DRL
     └── TCL
     
🔵 DDL (Data Definition Language)

Purpose
Used to define the structure of database objects.

Commands
CREATE
ALTER
DROP
TRUNCATE
Examples
CREATE TABLE student (...);
ALTER TABLE student ...;
DROP TABLE student;

🟢 DML (Data Manipulation Language)

Purpose
Used to manipulate data stored inside tables.

Commands
INSERT
UPDATE
DELETE
Examples
INSERT INTO student VALUES (...);
UPDATE student SET name='Mahesh';
DELETE FROM student;

🟡 DCL (Data Control Language)
Purpose
Used to control permissions and security.

Usually used by DBA users.

Commands
GRANT
REVOKE

Examples
GRANT CONNECT TO ramesh;
REVOKE CONNECT FROM ramesh;

🟣 DRL (Data Retrieval Language)
Purpose
Used to retrieve data from tables.

Command
SELECT
Example
SELECT * FROM student;

🔴 TCL (Transaction Control Language)
Purpose
Used to manage transactions.

Commands
COMMIT
ROLLBACK
Example
COMMIT;

Saves changes permanently.

ROLLBACK;

Undoes uncommitted changes.

🎯 Session–03 Summary

Learned Oracle user management.
Created users using CLI.
Granted permissions using GRANT.
Connected users using CONNECT.
Understood SQL Commands.
Learned the five categories of SQL commands:
DDL
DML
DCL
DRL
TCL

⚡ Quick Revision
Command Type	Purpose
DDL	Structure
DML	Data
DCL	Permissions
DRL	Retrieval
TCL	Transactions
Memory Trick
DDL → Design
DML → Modify Data
DCL → Control Access
DRL → Read Data
TCL → Transaction Control
