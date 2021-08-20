# Compass notes
*August 16th, 2021*
## Networking
---
### General
  * A (Computer) Network is when two or more computers are connected and can communicate with each other.
  * **TCP**, which stands for **Transmission Control Protocol**, provides a standard that allows machines to speak to each other.
  * **IP Address** - IP Address, which stans for **Internet Protocol Address**, is a unique address that identifies a device on the internet or a local network
  * **MAC Address** - **Media Access Control address** (MAC address) is a unique identifier assigned to a network interface controller (NIC)
  * **Port** - specific ports for each program on a computer, that allow them to network individually.
### `net` node module
  * You need to import the module `const net = require('net');`
  * Allows node to run servers apps and clients apps that can network with TCP
  * Not limited to languages, eg. Java server can use TCP with a python Client app
  * client is always the one establishing the connection to the server
  * client needs the destination IP address and PORT information
### Events and Event Handlers
  * change in the state of an object is known as an **Event** Can be something like, mouseclick, hover, key press, ect.
  * process of reacting over the events is called **Event Handling**. Usually a callback fnc, that executes when an event occurs
  ## HTTP HyperText Transfer Protocol
  ---
  * `HTTP` is the "language" that both client and server use to communicate over a TCP connection.
  * `HTTP` is a request-response based protocol. A client makes a request to an HTTP server, immediately also sending a message asking for a specific resource, which the server sends down as a response. A server cannot send a response to a client if the client has not first sent a request
  * `HTTP` Requests - Client wants to communicate with a server it issues a request
### HTTP Requests - Paths & Methods
  * `HTTP` has many components. Two of interests are **PATH** and **METHOD**
  * `GET`: used to "get" some data from the server
  * `POST`: usually used to create some new data
  * `PUT`: generally used for editing existing data on the server
  * `DELETE`: used to delete some existing data
### URL - Uniform Resource Locator
  * Protocol
  * Domain (or Host)
  * Port
  * Resource Path
  * Query Parameters
  * Anchor
  ### HTTP Responses - Status codes & Body
  * server wants to relay this information to a client it will use a status code
  * `200`: "Everything went great!"
  * `201`: "The request has succeeded and a new resource has been created as a result."
  * `404`: "Resource was not found."
  * `500`: "The server had an error
  * data is stored in a part of the response which is called the **body** This data can be text images, ect stored as HTML, encoded JSON, ect.