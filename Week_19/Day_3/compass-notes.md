# Compass Notes
*Nov 24th, 2021*
## Optimistic vs Pessimistic
  * async requests can be optimistic or pessimistic
  * optimistic is assuming the request will be successful, if not, update with an error
  * optimistic examples are likes, posting comments, other low important data flow
  * pessimistic is waiting for data to be successful before updating client's browser
  * pessimistic is a good choice for taxes, bank transactions
  * pessimistic is good for important data
## Reducers
  * The term reduce describes the process of taking multiple values and processing them one by one to create a single value. 
  * `Array.prototype.reduce` is a built in method for javascript for reduce.
  * React provides a Hook called `useReducer` that allows for more advanced state management patterns.
  * can use different patterns eg.
    * if conditions
    * switch/case
    * object lookup
  * In all scenarios, the important thing is that the reducer receives state and an action and can return the next state
## Web sockets
  * open a two-way interactive communication session between the user's browser and a server
  * uses webSocket protocol `ws://`, built on `TCP/IP`
  * low latency, persistent, full-duplex connection
  * use case examples: chat rooms, browser games, scheduling appointments