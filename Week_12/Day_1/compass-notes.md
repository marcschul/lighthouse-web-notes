# Compass notes
*Oct 4th 2021*
## Database Design
  * organization of data according to a database model
  * The designer determines what data must be stored and how the data elements interrelate
  * involves classifying data and identifying interrelationships
  * theoretical representation of the data is called an **ontology**
## Database Normalization
  * process of structuring a database with a series of normal forms
  * normal forms eg. 1Normal Form(`1NF`), 2Normal Form(`2NF`)
  * Reduces duplicate data
  * Involes creating more tables
  * Data highly space-efficient on disk
  * Enforce data integrity
  * Easier to manage data
  * database denormalized is the opposite, which stores data in multiple places
## Relationships Between Tables
  * Relationships between tables are based on primary keys(`PK`) and foreign keys(`FK`) Three main relationships are
    1. One-To-One
    2. One-To-Many
    3. Many-To-Many
  * Foreign Key(`FK`) is always on the many side
  * There are no direct many-to-many relationships, only multiple one-to-many relationships using a join table.
## ERD Entity Relationship Diagram
  * Always design a database using an ERD before writing any code.
  * Naming Convention
    * snake_case for table and column names
    * Pluralize tables names, column names should be singular
    * Call your primary key id
    * For most foreign keys use `<table>_id`
## Data Types
  * Many data types for efficiently storing data
  * If no data is provided for a column, the data type wil be `NULL`
## DDL Data Definition Language
  * commands define database schema referred as Data DDL statements 
    * `CREATE` - Creates a new entity
    * `ALTER` - Alters an entity
    * `DROP` - Deletes an entity
  * `DROP TABLE IF EXISTS users CASCADE;` is often used to delete all tables aswell as their children
## DML Data Manipulation Language
  * commands interact with data referred to as **DML**
    * `SELECT` get data from tables
    * `INSERT` add rows to a table
    * `UPDATE` update rows within a table
    * `DELETE` delete rows from a table
  * Not convention to delete data from our production database. Store data as 
  * Storage is not expensive
  * Never write an `UPDATE` or `DELETE` query without a `WHERE` clause.
