# Class 13

## Questions
1. What does it mean that web sockets are bidirectional? Why is this useful?

    This enables the server to send real-time updates asynchronously, without requiring the client to submit a request each time.
    
1. Does socket.io use HTTP? Why?

    Even when websockets can be used, the initial connection setup it done over HTTP. Also, a socket.io server will attach to an HTTP server so it can serve its own client code That said, although you don't need an HTTP server to regular websockets, there's no denying that the websocket protocol was designed with HTTP in mind.
1. What happens when a client emits an event?

    The event emitted from client side to server then it implement.
1. What happens when a server emits an event?

    The event emitted as many as server
1. What happens if a client “misses” an event?

    It doesn't happen.
1. How can we mitigate this?

    Sucket.


## Notes
1. Which 3 things had you heard about previously and now have better clarity on?
    * event
    * stacks
    * socket
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    * event
    * socket
    * Authentications
1. What are you most excited about trying to implement or see how it works?

    They will make our web page more dynamic.