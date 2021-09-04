# Compass notes
*September 2nd, 2021*
### REST - REpresentational State Transfer
  * a popular convention for structuring the routes in web applications.
  * set of conventions and practices in web development that deals with accessing and manipulating resources over HTTP
  * When an API conforms to REST, the API is known as a RESTful API
    * Example: GitHub API is RESTful. It can be used to manage resources such as Users, Repos, Commits, Gists, and so forth. Each resource can be accessed using an API endpoint (which is simply a URL).

### Resource
  * can be a document, a photo, or anything else
  * an abstraction of an object or data
  * referenced using a URL (Uniform Resource Locator).
  * Perfom various operations on these resources (create, delete, modify) using the different HTTP methods

### BREAD
  | Action | Application | Description | HTTP Method |
  |--------|-------------|-------------|-------------|
  | B | 2 | 3 | 4 |
  | Browse |collection |	browse the collection |	GET|
  | Read |	member |	read a member of the collection |	GET|
  | Edit | 	member |	edit a member of the collection |	PUT / PATCH|
  | Add |	collection |	add a new member to the collection |	POST|
  | Delete |	member |	delete a member of the collection |	DELETE|

### Resource Identifier

  * identifying a resource, "naming it" 
  * Naming convention is object type, plural, all lower case, words separated with hyphens
  * example
    * user's collection would be identified as `/user`
    * user's first member would be identified as `/user/1`
