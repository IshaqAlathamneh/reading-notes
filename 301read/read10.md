# Read-10

### Call stack
A call stack is a mechanism for an interpreter to keep track of its place in a script that calls multiple functions what function is currently being run and what functions are called from within that function.

*In summary, then, we start with an empty Call Stack. Whenever we invoke a function, it is automatically added to the Call Stack. Once the function has executed all of its code, it is automatically removed from the Call Stack. Ultimately, the Stack is empty again.*

At the most basic level, a call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

***Why call stack?*** 

The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.

***Temporarily store:*** When a function is invoked (called), the function, its parameters, and variables are pushed into the call stack to form a stack frame. This stack frame is a memory location in the stack. The memory is cleared when the function returns as it is pop out of the stack.

***What causes a stack overflow?***
A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

### summary
The key takeaways from the call stack are:
1. It is single-threaded. Meaning it can only do one thing at a time.
2. Code execution is synchronous.
3. A function invocation creates a stack frame that occupies a temporary memory.
4. It works as a LIFO — Last In, First Out data structure.

#### Types of error messages
* Reference errors
This is as simple as when you try to use a variable that is not yet declared you get this type os errors.
* Syntax errors
I know it’s in the name of the errors, but like it says itself, this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.
* Range errors
Like you give a nigative length to an array
* Type errors
Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

#### Debugging
To debug your JS code, the easiest and maybe the most common way its to simply console.log() the variables you want to check or, by using chrome developer tools, open your page with your JS code  and choose your file to debug, click the line you wanna debug and refresh your page again .
If the line you selected was run you will be able to see what has happened before that point and you can try and evaluate the next lines to check if everything is outputting what you are expecting.
The breakpoint can also be achieved by putting a debugger statement in your code in the line you want to break.

#### Handling errors

An alternative it’s to encapsulate our problematic function code with a try…catch which would make an error be thrown but this time, not “uncaught” so we can send it to a error logging to be checked later and send a fallback to the function so that our code continues without problems.
