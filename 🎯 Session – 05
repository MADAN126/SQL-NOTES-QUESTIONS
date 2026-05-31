2022

🔄 Previous Session Recap (Session–04)
Learned about Database Tables.
Created tables using the CREATE command.
Understood Oracle Naming Conventions.
Inserted records using the INSERT command.
Retrieved records using the SELECT command.
Learned the basic flow:
CREATE TABLE
      ↓
INSERT DATA
      ↓
SELECT DATA

📖 Current Session Topics
SQL*Plus Useful Commands
UPDATE Statement
Updating All Rows
Updating Particular Rows
WHERE Clause
DELETE Statement
Deleting All Rows
Deleting Particular Rows

1️⃣ Useful SQL*Plus Commands
Clear Screen

To clear the SQL*Plus screen:
CL SCR;

Increase Line Width
To display more characters in one line:

SET LINESIZE 300;

Purpose
Prevents output from wrapping into multiple lines.

2️⃣ UPDATE Statement

What is UPDATE?

The UPDATE command is used to modify existing records in a table.

Category
DML (Data Manipulation Language)
Real-Life Example

Suppose customer Mahesh moved from Hyderabad to Pune.

Old Record:

ID	Name	Location
1	Mahesh	Hyderabad

After Update:

ID	Name	Location
1	Mahesh	Pune
3️⃣ Updating All Rows

If WHERE condition is not specified, Oracle updates every row in the table.

Syntax
UPDATE table_name
SET column_name = value;
Example

Update all customers' location to Delhi.

UPDATE ashokit_customers
SET location='Delhi';
Output
3 rows updated.
Before Update
ID	Name	Location
1	Mahesh	Hyderabad
2	Ashok	Hyderabad
3	Rajesh	Mumbai
After Update
ID	Name	Location
1	Mahesh	Delhi
2	Ashok	Delhi
3	Rajesh	Delhi
⚠ Important Rule
No WHERE Clause
       ↓
All Rows Updated

Always be careful while using UPDATE.

4️⃣ Updating Particular Rows

To update specific records, use the WHERE clause.

Syntax
UPDATE table_name
SET column_name = value
WHERE condition;
Example 1

Update location to Pune for customer_id = 1

UPDATE ashokit_customers
SET location='Pune'
WHERE customer_id=1;
Output
1 row updated.
Example 2

Update location based on customer name.

UPDATE ashokit_customers
SET location='Pune'
WHERE customer_name='Mahesh';
Example 3

Update multiple columns.

UPDATE ashokit_customers
SET location='Guntur',
    age=40
WHERE customer_name='Mahesh';
Example 4

Using Multiple Conditions

UPDATE ashokit_customers
SET location='Guntur',
    age=40
WHERE customer_name='Mahesh'
AND gender='Male';
5️⃣ Understanding WHERE Clause
Purpose

The WHERE clause is used to select specific rows.

Syntax
WHERE condition
Examples
WHERE customer_id=1
WHERE customer_name='Mahesh'
WHERE age > 30
WHERE gender='Male'
AND age>=35
💡 Real-Time Recommendation

Always update records using:

customer_id

instead of:

customer_name
Why?

Customer IDs are unique.

Names may be duplicated.

Example:

ID	Name
1	Mahesh
5	Mahesh

Updating by name may affect multiple rows.

Updating by ID affects only one row.

6️⃣ DELETE Statement
What is DELETE?

DELETE is used to remove records from a table.

Category
DML (Data Manipulation Language)
7️⃣ Deleting All Rows

If WHERE clause is omitted, all records will be deleted.

Syntax
DELETE FROM table_name;
Example
DELETE FROM ashokit_customers;
Result
All rows deleted.
⚠ Important Rule
No WHERE Clause
       ↓
All Rows Deleted

Be extremely careful.

8️⃣ Deleting Particular Rows

To delete specific records, use WHERE clause.

Syntax
DELETE FROM table_name
WHERE condition;
Example 1

Delete customer with ID = 1

DELETE FROM ashokit_customers
WHERE customer_id=1;
Example 2

Delete customer named Ashok

DELETE FROM ashokit_customers
WHERE customer_name='Ashok';
Example 3

Delete all male customers

DELETE FROM ashokit_customers
WHERE gender='Male';
Example 4

Delete male customers whose age is greater than or equal to 35

DELETE FROM ashokit_customers
WHERE gender='Male'
AND age>=35;
🎯 Difference Between UPDATE and DELETE
UPDATE	DELETE
Modifies existing data	Removes data
Rows remain	Rows are removed
Uses SET keyword	Does not use SET
Can use WHERE	Can use WHERE
🎯 Session Summary
UPDATE

Used to modify existing records.

UPDATE table_name
SET column=value
WHERE condition;
DELETE

Used to remove records.

DELETE FROM table_name
WHERE condition;
Keywords Learned
Keyword	Purpose
UPDATE	Modify Data
SET	Specify New Values
WHERE	Apply Conditions
DELETE	Remove Data
❓ Interview Questions
Q1. Which command is used to modify records?

UPDATE

Q2. Which command is used to delete records?

DELETE

Q3. What happens if UPDATE is used without WHERE?

All rows are updated.

Q4. What happens if DELETE is used without WHERE?

All rows are deleted.

Q5. Which keyword is used to specify conditions?

WHERE

Q6. Why is customer_id preferred in UPDATE statements?

Because it is unique for every customer.

⚡ Quick Revision Sheet
Command	Purpose
CREATE	Create Table
INSERT	Add Records
SELECT	Retrieve Records
UPDATE	Modify Records
DELETE	Remove Records
Golden Memory Rule
CREATE
   ↓
INSERT
   ↓
SELECT
   ↓
UPDATE
   ↓
DELETE
