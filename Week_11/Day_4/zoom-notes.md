# Zoom notes
*September 30th, 2021*
## notes
  * Review
  * Database
  * Terminology
  * ERD
  * Relations
  * ERD
  * Best Practice
  * Breakout
  * Solve ERD together
## Keys
  * Primary Key
    * must be unique
    * any datatype
    * Are indexed columns
  * 
## Conventions
  * Tables are labelled plural eg. `Users`
  * FK are singular eg. `User_ID`
  * PK, Primary Key, eg. `id (PK)`
  * FK, Forgein Key, eg. `id (FK)`
  * `FK` is always on the many side
  * `FK` cannot be null, throws an error
  * www.draw.io
  * `CASCADE DELETE` -> Deletes parents and it's children
  * often, records are active / deactive, not deleted. often referenced as `active` column
  * record often have `created` and `updated` columns

## SQL Data types
  * A lot of data types
    * integer
    * varchars
    * booleans
    * text
    * date
    * timestamp
    * ect...

## Relationships
  * one to many
  * many to one
  * many to many
    * requires more than two tables, often called `bridge table`.
    * `bridge table` often labelled by action `eg.` restaraunt and diner tables may label their `bridge table`, "meals".
    * requires one-too-many to bridge to one-too-many