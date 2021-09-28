# Compass notes
*September 27th, 2021*
## Databases
  * organized collection of structured data
  * organized
  * searchable
  * reliable
  * easy to update
  * secure
  * avoid redundancy
  * searchable
  * different kinds of databases
## DBMS - Database Management Software
  * software designed to store, retrieve, define, and manage data in a database.
  * e.g MySQL, Oracle, PostgreSQL, FoxPro
## Database Types
  * Document db
  * Key-value stores
  * Column-oriented db
  * Graph db
  * relational db
## Relational Databases
  * `Rows` === `Records`
  * `Columns` === `Fields`
  * Databases can have more than 1 table
  * Structure of a table in the database is called the schema
  * May provide unique values to data, to avoid duplications

  | Field#1 or Column#1 | Field or Column#2 | Field or Column#3 |
  |---|---|---|
  | Record or Row#1 | Data |  Data |
  | Rocord or Row#2 | Data |  Data |
## Relationships
  * connects data to each way to use in more complex and realistic ways
  * connects two pieces of data in different tables in the same database
  * One-to-many
  * Many-to-many
  * One-to-one
## Transactions
represents any change in a database
### ACID
A method for handling transactions, usually handled by DBMS automatically.
  * **A**tomic - cannot be divided
  * **C**onsistent - cannot violate integrity rules
  * **I**solated - one transaction at a time
  * **D**urable - written to the db, and waits for completion
## SQL - Structured Query Language
  * Many versions, MySQL, T-SQL, ect.
  * Users write statements
  * Features to manage database. 
  * the standard language for working with RDBMSs
  * SQL Satement has Clauses, Keywords, Predicates, Expressions
  * UPPER CASE not required but is a convention for `keywords`
  ```sql
  /* SQL Statement */
  WHERE LastName = 'Schulmeister';
  /*
  * Clause
  * WHERE LastName = 'Schulmeister';
  *
  * Keyword
  * WHERE
  * 
  * Predicate
  * 'Schulmeister'
  *
  * Expression
  * 'Schulmeister'
  */
  ```
## RDBMS - Relational database management systems
  * software that let you create and use relational databases
  * eg. mySQL, SQLite, PostgreSQL, IBM DB2, Oracle Database
  * RDBMSs require that each column in a table is given a data type
## ERD - Entity Relationship Diagram
5 Main parts of the diagram
  1. **Entities** - a person, place, or thing in the database. Each occurance is an entity instance, othewise known as "table".
  2. **Attributes** - describes various characteristics about an individual entity. "columns" in the table
  3. **Primary Key** - An attribute or group of attributes that uniquely identifies an instance of the entity
  4. **Relationship** - Describes how one or more entities interact with each other
  5. **Cardinality** - The count of instances that are allowed or are necessary between entity relationships