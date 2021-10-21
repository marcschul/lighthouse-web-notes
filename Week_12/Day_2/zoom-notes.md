# Zoom notes
*October 5th, 2021*
## SQL from Apps
  * review the online library database
  * `BREAD` or `CRUD` actions on database via command line app
  * Avoid SQL injection attack
  * Serve database content to the browser(client)
  * Protect secrets with environment variables
## SQL Injection Attacks
  * AVOID using template literal placeholders. Vunerable to SQL Injection attacks
  * User input's code as a value for malicous purposes
  * node-PostgresSQL provides `Parameterized query` to defened SQL Injection atatcks
## Environment variables
  * dynamic-named value that can affect the way running processes will behave on a computer