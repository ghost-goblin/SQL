# 🏓 Structured Query Language
SQL is a standard language for storing, manipulating and retrieving data in databases.

## Syntax Rules
```sql
-- The following SQL statement selects all the columns from the "table_name" table:
SELECT * FROM table_name;

-- The following SQL statement selects the "column1" and "column2" columns from the "table_name" table:
SELECT column1, column2 FROM table_name;
```

> SQL keywords are NOT case sensitive: `select` is the same as `SELECT`

+ The `WHERE` clause is used to filter records and extract only those records that fulfill a specified condition.

```sql
SELECT column1, column2. ...
FROM table_name WHERE condition;
```

## Relational Database Management System
**RDBMS** is the basis for SQL and the data in RDBMS is stored in database objects called tables. **RDBMS** uses a structure that allows us to identify and access data _in relation_ to another piece of data in the database. A table is a collection of related data entries and it consists of columns and rows (often called _records_).
A database most often contains one or more tables. Each table is identified by a name (e.g. "Customers" or "Products").

## Postgres
A powerful and open source **object-relational database** where you can model any data and their relationships using tables, keys, constaints and triggers.
Postgres itself is a database _server_ and there are several ways to connect to the database; **GUI**s, **CLI**s and **ORM**s (**Object–Relational Mapping**, a programming technique for converting data between incompatible types of systems by creationg a "virtual object database" using object-oriented programming languages).
In order to run and use Postgres on your own computer, you will need to set up both a Postgres server and a client.

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
