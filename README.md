# 🏓 [Structured Query Language](https://www.w3schools.com/Sql/default.asp)
**SQL** is a standard language for _storing_, _manipulating_ and _retrieving_ data in databases.

## Syntax Rules
```sql
-- The following SQL statement selects all the columns from the "table_name" table:
SELECT * FROM table_name;

-- The following SQL statement selects the "column1" and "column2" columns from the "table_name" table:
SELECT column1, column2 FROM table_name;
```

> SQL keywords are NOT case sensitive: `select` is the same as `SELECT`

### The `WHERE` clause is used to filter records and extract only those records that fulfill a specified condition:

```sql
SELECT column1, column2. ...
FROM table_name WHERE condition;
```
+ The `WHERE` clause can be conbined with `AND`, `OR` and `NOT` operators.

### A `JOIN` clause is used to combine rows from two or more tables, based on a related column between them:

Here are the different types of the JOINs in SQL:
+ `(INNER) JOIN`: Returns records that have matching values in both tables
+ `LEFT (OUTER) JOIN`: Returns all records from the left table, and the matched records from the right table
+ `RIGHT (OUTER) JOIN`: Returns all records from the right table, and the matched records from the left table
+ `FULL (OUTER) JOIN`: Returns all records when there is a match in either left or right table

### Create a new database:
 ```sql
 CREATE DATABASE databasename;
 ````
### Create a new table in a database:
```sql
CREATE TABLE table_name (
  column1 datatype,
  column2 datatype.
  column3 datatype,
  ...
);
```
_Let's see an example, shall we?_
```sql
CREATE TABLE Humans (
  PersonID int,
  LastName varchar(255),
  FirstName varchar(255),
  Address varchar(255),
  City varchar(255)
);
```
If you [click here](https://www.w3schools.com/Sql/sql_datatypes.asp), you can have a look at all the SQL data types. Spoiler Alert; there's a lot! 😱

> Each column in a database table is required to have a name and a data type.

### The `ALTAR` statement is used to add, delete, or modify columns in an existing table:
```sql
ALTER TABLE table_name
ADD column_name datatype;
```

### SQL Constaints are used to specify rules for data in a table and can be specified when the table is created with the `CREATE TABLE` or the `ALTER TABLE` statement:
```sql
CREATE TABLE table_name (
    column1 datatype constraint,
    column2 datatype constraint,
    column3 datatype constraint,
    ....
);
```
Constaints are used to limit the type of data that goes into a table which ensures accuracy and reliability of the data. Constaints can be column level or table level.
The commonly used constaints are:
+ `NOT NULL` - Ensures that a column cannot have a NULL value
+ `UNIQUE` - Ensures that all values in a column are different
+ `PRIMARY KEY` - A combination of a NOT NULL and UNIQUE. Uniquely identifies each row in a table
+ `FOREIGN KEY` - Prevents actions that would destroy links between tables
+ `CHECK` - Ensures that the values in a column satisfies a specific condition
+ `DEFAULT` - Sets a default value for a column if no value is specified
+ `CREATE INDEX` - Used to create and retrieve data from the database very quickly


* * *

## Relational Database Management System
**RDBMS** is the basis for SQL and the data in RDBMS is stored in database objects called tables. **RDBMS** uses a structure that allows us to identify and access data _in relation_ to another piece of data in the database. A table is a collection of related data entries and it consists of columns and rows (often called _records_).
A database most often contains one or more tables. Each table is identified by a name (e.g. "Customers" or "Products").

* * *

## [Postgres](https://www.postgresql.org/)
A powerful and open source **object-relational database** where you can model any data and their relationships using _tables_, _keys_, _constaints_ and _triggers_.
Postgres itself is a database _server_ and there are several ways to connect to the database; **GUI**s, **CLI**s and **ORM**s (**Object–Relational Mapping**, a programming technique for converting data between incompatible types of systems by creationg a _"virtual object database"_ using object-oriented programming languages).
In order to run and use Postgres on your own computer, you will need to set up both a Postgres server and a client.

* * *

## Some of The Most Important SQL Commands
* `SELECT` - extracts data from a database
* `UPDATE` - updates data in a database
* `DELETE` - deletes data from a database
* `INSERT INTO` - inserts new data into a database
* `CREATE DATABASE` - creates a new database* 
* `ALTER DATABASE` - modifies a database
* `CREATE TABLE` - creates a new table
* `ALTER TABLE` - modifies a table
* `DROP TABLE` - deletes a table
* `CREATE INDEX` - creates an index (search key)
* `DROP INDEX` - deletes an index
