# Compass notes
*August 24th, 2021*
## General
### CRUD
  * Allows users to manipulate data
  * **C**reate - add new record
  * **R**ead - retrieve value of record
  * **U**pdate - Update record's value
  * **D**elete Delete record

|Action|JavaScript|
|---|---|
Create|`users["5315"] = {first_name: "John", last_name: "Smith"}`
Read|`users["5315"]`
Update|`users["5315"].first_name = "Jane"`
Delete|`delete users["5315"]`

HTTP was designed around the concept of resources (described by URLs) and actions that can be taken on them. To take an action on a resource, a client (for example, a browser) sends an HTTP request to a server with the appropriate URL and method. The following table shows how the most common HTTP methods correspond with CRUD actions.

|HTTPMethod|CRUD Action|
|---|---|
`GET`|Read
`POST`|Create
`PUT`|Update
`DELETE`|Delete