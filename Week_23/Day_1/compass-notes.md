# Compass Notes
*Jan 3rd, 2022*
## Ruby on Rails
  * Rails is a model–view–controller (MVC) framework, providing default structures for a database, a web service, and web pages.

## Ruby's Active Record - AR
  * Active Record is the M in MVC - **model**, view, controller
  * Facilitates the creation and use of business objects whose data requires persistent storage to a database.
  * Model Class - Singular with the first letter of each word capitalized
    * e.g: `BookClub`
  * Database Table - Plural with underscores separating words
    * e.g: `book_clubs`
  * Foreign keys - These fields should be named following the pattern singularized_table_name_id e.g. `item_id` , `order_id`. These are the fields that Active Record will look for when you create associations between your models.
  * Primary keys - By default, Active Record will use an integer column named id as the table's primary key (bigint for PostgreSQL and MySQL, integer for SQLite). When using Active Record Migrations to create your tables, this column will be automatically created.
  * Active Record `callbacks` allow you to attach code to certain events in the life-cycle of your models.
  * 


## MVC - Model View Controller
repeating pattern 1 to 8
  1. model
  2. updates
  3. view
  4. sees
  5. user
  6. uses
  7. controller
  8. manipulate