🔄 Previous Session Recap (Session–05)
Learned DML Commands:
INSERT
UPDATE
DELETE
Modified existing records using UPDATE.
Deleted records using DELETE.
Understood the importance of the WHERE clause.
Learned SQL*Plus commands:
CL SCR
SET LINESIZE
Practiced table creation and data manipulation.

📖 Current Session Topics
What is a Datatype?
Number Datatypes
Character Datatypes
Date Datatype
Timestamp Datatype
Large Object Datatypes (CLOB, BLOB, BFILE)
Creating Employee Table
Inserting Data into Table
DESCRIBE Command

1️⃣ What is a Datatype?

Definition
A Datatype defines the type of value that can be stored in a database column.

Why Datatypes?

Datatypes ensure that only valid data is stored.

Example
Column	Datatype	Value
EmpId	  NUMBER	  101
EmpName	VARCHAR2	Mahesh
Gender	CHAR    	M
DOB	    DATE	    24-APR-2004

🏛 Oracle Datatype Categories

Oracle classifies datatypes into:

Oracle Datatypes
      │
      ├── Number
      ├── Character
      ├── Date
      ├── Timestamp
      └── Miscellaneous
2️⃣ NUMBER Datatype

Used to store numeric values.

Types of Numbers
Whole Numbers
10
20
55
100
9999
Decimal Numbers
10.25
99.99
123.456
5000.75

A) NUMBER(size)

Stores only integer values.

Syntax

column_name NUMBER(size)

Example
student_no NUMBER(4)

Meaning

Maximum 4 digits allowed.

9999 ✔
1000 ✔
12345 ❌

B) NUMBER(precision, scale)

Used for decimal values.

Syntax
column_name NUMBER(precision, scale)
Important Terms
Precision

Total number of digits.

Scale

Digits after the decimal point.

Example
salary NUMBER(6,2)

Maximum Value:

9999.99

Explanation:

Total Digits = 6
Decimal Digits = 2
Example
bill_amount NUMBER(8,3)

Maximum Value:

12345.678

Real-Time Usage
Employee Salary
Product Price
Bank Interest Rate
Customer Bill Amount

3️⃣ Character Datatypes

Used to store alphabetic and textual data.

A) CHAR(size)

Stores fixed-length character data.

Syntax
column_name CHAR(size)

Example
student_name CHAR(25)
Characteristics

✅ Maximum Size: 2000 Characters

✅ Fixed-Length Storage

✅ Static Memory Allocation

Example
CHAR(10)

Value = 'RAM'

Oracle reserves all 10 characters.

RAM_______

(remaining space filled internally)

Best Usage
Gender
Status
Grade
Country Codes

B) VARCHAR / VARCHAR2

Stores variable-length character data.

Syntax
column_name VARCHAR2(size)

Example
student_name VARCHAR2(30)
Characteristics

✅ Maximum Size: 4000 Characters

✅ Dynamic Memory Allocation

✅ Uses only required space

Example
VARCHAR2(10)

Value = 'RAM'

Stores only:

RAM

No extra memory wasted.

VARCHAR vs VARCHAR2
VARCHAR	VARCHAR2
SQL Standard	Oracle Specific
Less commonly used	Most commonly used
Developed by SQL Standard	Developed by Oracle
Interview Tip

Always prefer:

VARCHAR2

in Oracle projects.

4️⃣ DATE Datatype

Used to store date values.

Examples
Date of Birth
Hire Date
Joining Date
Booking Date
Purchase Date

Syntax
column_name DATE

Example
dob DATE

Default Oracle Date Format
DD-MON-YY

Examples
12-FEB-13
24-APR-04
18-SEP-15

5️⃣ TIMESTAMP Datatype

Stores both Date and Time.

Syntax
column_name TIMESTAMP

Example
created_dt TIMESTAMP
Default Format
DD-MON-YY HH:MI:SS

Example
30-NOV-22 10:01:20 PM
Real-Time Usage
Audit Logs
Transaction History
Login Tracking
Record Creation Time

6️⃣ Miscellaneous Datatypes

Used for storing large amounts of data.

A) CLOB
Character Large Object

Stores very large text data.

Capacity
1 GB – 4 GB

Examples
Articles
Documentation
Books
Reports

B) BLOB
Binary Large Object

Stores binary data.

Capacity
1 GB – 4 GB

Examples
Images
Videos
Audio Files
PDF Documents
C) BFILE
Binary File

Stores references to external files.

Capacity
1 GB – 4 GB
Examples
External Documents
Media Files
Binary Files

7️⃣ Creating Employee Table

Table Structure
CREATE TABLE ashokit_employees(
    empId NUMBER(5),
    empName VARCHAR2(50),
    gender CHAR(1),
    dob DATE,
    created_dt TIMESTAMP
);

Column Analysis

Column	    Datatype	    Purpose
empId	      NUMBER(5)	    Employee ID
empName	    VARCHAR2(50)	Employee Name
gender	    CHAR(1)	      Gender
dob	        DATE	        Date of Birth
created_dt	TIMESTAMP	    Record Creation Time

8️⃣ Inserting Data

Example
INSERT INTO ashokit_employees
VALUES(5656,'Rani','F','24-APR-2004',SYSDATE);

Another Example

INSERT INTO ashokit_employees
VALUES(5657,'Ramesh','M','24-APR-2004',SYSDATE);

What is SYSDATE?

SYSDATE returns the current system date and time.

Example
SYSDATE

Output:

30-NOV-22 10:01:20 PM
9️⃣ Viewing Table Structure
DESCRIBE Command

Used to display table structure.

Syntax
DESC table_name;
Example
DESC ashokit_employees;
Output
Column	Datatype
EMPID	NUMBER(5)
EMPNAME	VARCHAR2(50)
GENDER	CHAR(1)
DOB	DATE
CREATED_DT	TIMESTAMP(6)
🎯 Session Summary
Number Datatypes
NUMBER(size)
NUMBER(precision, scale)
Character Datatypes
CHAR(size)
VARCHAR2(size)
Date Datatypes
DATE
TIMESTAMP
Large Object Datatypes
CLOB
BLOB
BFILE
Important Commands
CREATE TABLE
INSERT INTO
SELECT *
DESC
❓ Interview Questions
Q1. What is a Datatype?

A datatype defines the type of value that can be stored in a database column.

Q2. Difference between NUMBER(5) and NUMBER(5,2)?
NUMBER(5) → Integers
NUMBER(5,2) → Decimal Values
Q3. Difference between CHAR and VARCHAR2?
CHAR → Fixed Length
VARCHAR2 → Variable Length
Q4. What is Oracle's default date format?
DD-MON-YY
Q5. Which datatype stores date and time?
TIMESTAMP
Q6. What is SYSDATE?

Returns the current system date and time.

Q7. Which command displays table structure?
DESC table_name;
⚡ Quick Revision Sheet
Datatype	Purpose
NUMBER	Numeric Values
CHAR	Fixed Text
VARCHAR2	Variable Text
DATE	Date Only
TIMESTAMP	Date + Time
CLOB	Large Text
BLOB	Binary Data
BFILE	External Files
Golden Memory Rule
NUMBER      → Numbers
VARCHAR2    → Text
DATE        → Date
TIMESTAMP   → Date + Time
CLOB/BLOB   → Large Data
