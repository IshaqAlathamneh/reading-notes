# Read 10

## ERROR HANDLING & DEBUGGING

#### ORDER OF EXECUTION
The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run.

#### EXECUTION CONTEXTS
The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new execution context. They correspond to variable scope. 
1. GLOBAL CONTEXT
1. GLOBAL SCOPE
1. EVAL CONTEXT (NOT SHOWN)

#### THE STACK
The JS interpreter processes one line of code at a time. When statment needs data from another function it stacks the new function on top of the current task.

#### EXECUTION CONTEXT & HOISTING
1. PREPARE
* The new scope is created
* Variables, functions, and arguments are created
* The value of the this keyword is determined
1. EXECUTE 
* Now it can assign values to variables
* Reference functions and run their code
* Execute statements

#### UNDERSTANDING SCOPE
In the interpreter, each execution context has its own variables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent's variables object. 

#### UNDERSTANDING ERRORS 
If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handl ing code.

#### HOW TO DEAL WITH ERRORS
1. DEBUG THE SCRIPT TO FIX ERRORS 
If you come across an error while writing a script, you will need to debug the code, track down the source of the error, and fix it.
1. HANDLE ERRORS GRACEFULLY
You can handle errors gracefully using try, catch, throw, and f i na 1 ly statements.

***WHERE IS THE PROBLEM?***
1. Look at the error message, it tells you:
* The relevant script that caused the problem.
* the line number
* The type of error
1. . Check how far the script is running.
1. Use breakpoints where things are going wrong. They let you pause execution and inspect the values that are stored in variables.

***WHAT EXACTLY IS THE PROBLEM? ***
1. When you have set breakpoints, you can see if the variables around them have the values you would expect them to. If not, look earlier in the script.
1. Break down I break out parts of the code to test smaller pieces of the functionality.
* Write values of variables into the console. 
* Calrfunctions from the console
* Check if objects exist and have the methods I properties that you think they do.
1. Check the number of parameters for a function, or the number of items in an array

***The JavaScript console will tell you when there is a problem with a script, where to look for the problem, and what kind of issue it seems to be. ***

#### BREAKPOINTS
* You can pause the execution of a script on any line using breakpoints. Then you can check the values stored in variables at that point in time. 
* If you set multiple breakpoints, you can step through them one-by-one to see where values change and a problem might occur. 

#### CONDITIONAL BREAKPOINTS
You can indicate that a breakpoint should be triggered only if a condition that you specify is met. The condition can use existing variables.

***You can create a breakpoint in your code using just the debugger keyword.***

* It is particularly important to remember to remove these statements before your code goes live as this could stop the page running if a user has developer tools open.
* If you know your code might fail, use try, catch, and finally. Each one is given its own code block.
* If you know something might cause a problem for your script, you can generate your own errors before the interpreter creates them.
* Debugging is the process of finding errors. It involves a process of deduction.

#### COMMON ERRORS
* GO BACK TO BASICS: JavaScript is case sensitive so check your capitalization.
* MISSED/ EXTRA CHARACTERS: Every statement should end in a semicolon. 
* DATA TYPE ISSUES: Using= rather than == will assign a value to a variable, not check that the values match.