# Restaurant RESTful API
This API allows you to view and order food from a restaurant  
The API uses JSON format  
This API is available at localhost:8080/api

## API Routes
---

/customers  
/customer  
/menu_items  
/tickets  
/ticket  
/locations  
/location  

<br>

## Endpoints
---

<br>

### Customer's Information
---
`GET /customers`  
returns an object of all customers with their information  

`GET /customer/:id`  
returns a specific customer given their customer id  

`POST /customer`  
handles a request to add an individual customer to db  

`PUT /customer/:id`  
handles a request to update individual customer in db  

<br>

### Menu
---
`GET /menu_items`  
returns an object with nested objects of available food  

<br>

### Food Tickets
---
`GET /tickets`  
returns a full list of tickets  

`GET /ticket/:id`  
returns a specific ticket  

`POST /ticket/:id`  
handles a request to add new ticket  

`PUT /ticket/:id`  
handles a request to update individual ticket in db  

<br>

### Store Locations
---
`GET /locations`  
returns a list of all restaurants  

`GET /location/:id`  
returns a specific restaurant's information  

`POST /location/:id`  
handles a request to create a new restaurant  

`PUT /location/:id`  
handles a request to update an individual restaurant's information in  server's db
