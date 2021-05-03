# Class 03

## Questions
1. Name 3 real world use cases where you’d want to change the request with custom middleware

    * Registering middleware (log in)
    * Duplicating Data: We can store duplicate data in our search server so it can directly search them instead of requesting from product and user servers. 
    * API Security: We talked about a User server that takes care of the login and sign-up. If our front end code directly sends the requests to that server, the address of our authentication server is exposed. After learning the IP address of our backend, attackers can use tools to find our endpoints and scan our server for vulnerabilities.
1. True or false: The route handler is middleware?
    True
1. In what ways can a middleware function end the process and send data to the browser?

    if there's an error or the next fubction invoke with arguments
1. At what point in the request lifecycle can you “inject” middleware?
     at the beggining of the requests
1. What can cause express to error with “Request headers sent twice, cannot start a second response”
     means that you're already in the Body or Finished state.

## Notes
1. Which 3 things had you heard about previously and now have better clarity on?
    * node.js
    * npm
    * express
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    * http status codes
    * express methods
    * ES6 Classes
1. What are you most excited about trying to implement or see how it works?

    thinking how they will make you experience much easier.