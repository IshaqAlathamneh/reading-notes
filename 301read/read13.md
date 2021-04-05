# Read-13

#### Sending form data
First we'll discuss what happens to the data when a form is submitted.

#### Client/server architecture
At it's most basic, the web uses a client/server architecture that can be summarized as follows. a client sends a request to a server , using the HTTP protocol. The server answers the request using the same protocol.
An HTML form on a web page is nothing more than a convenient user-friendly way to configure an HTTP request to send data to a server. This enables the user to provide information to be delivered in the HTTP request.

#### On the client side: defining how to send the data
The `<form>` element defines how the data will be sent. All of its attributes are designed to let you configure the request to be sent when a user hits a submit button. The two most important attributes are action and method.
The action attribute defines where the data gets sent. and The method attribute defines how data is sent.

The GET method is the method used by the browser to ask the server to send back a given resource.
The POST method is a little different. It's the method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request.

#### Viewing HTTP requests
1. Open the developer tools.
1. Select "Network"
1. Select "All"
1. Select "foo.com" in the "Name" tab
1. Select "Headers"

#### On the server side: retrieving the data
Whichever HTTP method you choose, the server receives a string that will be parsed in order to get the data as a list of key/value pairs. The way you access this list depends on the development platform you use and on any specific frameworks you may be using with it.

#### Security issues
Each time you send data to a server, you need to consider security. HTML forms are by far the most common server attack vectors (places where attacks can occur). The problems never come from the HTML forms themselves — they come from how the server handles data.

#### Summary
As we'd alluded to above, sending form data is easy, but securing an application can be tricky. Just remember that a front-end developer is not the one who should define the security model of the data.It's possible to perform client-side form validation, but the server can't trust this validation because it has no way to truly know what has really happened on the client-side.

### You Can Read More About HTML Forms By [Clicking Here](https://htmlreference.io/forms/)