# Read-06

## What Is Node and When Should I Use It?

#### What Is Node.js?
There are plenty of definitions to be found online. Let’s take a look at a couple of the more popular ones. This is what the project’s home page has to say: `Node.js® is a JavaScript runtime built on Chrome’s V8 JavaScript engine.`
And this is what Stack Overflow has to offer: `Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.`

#### Node Is Built on Google Chrome’s V8 JavaScript Engine
The V8 engine is the open-source JavaScript engine that runs in Google Chrome and other Chromium-based web browsers, including Brave, Opera, and Vivaldi. It was designed with performance in mind and is responsible for compiling JavaScript directly to native machine code that your computer can execute.

### How Do I Install Node.js?
In this next section, we’ll install Node and write a couple of simple programs. We’ll also look at npm, a package manager that comes bundled with Node.

#### Node Binaries vs Version Manager
Many websites will recommend that you head to the official Node download page and grab the Node binaries for your system.
While that works, I would suggest that you use a version manager instead. This is a program that allows you to install multiple versions of Node and switch between them at will.
#### “Hello, World!” the Node.js Way
You can check that Node is installed on your system by opening a terminal and typing `node -v` you should see something like `v12.14.1`
Next, create a new file `hello.js` and copy in the following code: `console.log("Hello, World!");`
This uses Node’s built-in console module to display a message in a terminal window. To run the example, enter the following command: `node hello.js` If Node.js is configured properly, “Hello, World!” will be displayed.


***Node.js Has Excellent Support for Modern JavaScript***

the package manager for JavaScript, npm is also the world’s largest software registry. There are over 1,000,000 packages of JavaScript code available to download, with billions of downloads per week. Let’s take a quick look at how we would use npm to install a package.

#### Installing a Package Globally
Open your terminal and type the following:

`npm install -g jshint`
This will install the jshint package globally on your system. We can use it to lint the `index.js` file from the previous example:

`jshint index.js`
You should now see a number of ES6-related errors. If you want to fix them up, add `/* jshint esversion: 6 */` to the top of the `index.js` file, re-run the command and linting should pass.

#### Installing a Package Locally
We can also install packages locally to a project, as opposed to globally, on our system. Create a `test` folder and open a terminal in that directory. Next type this:

`npm init -y`
This will create and auto-populate a `package.json` file in the same folder. Next, use npm to install the lodash package and save it as a project dependency:

`npm install lodash --save`
Create a file named `test.js` and write your code
Finally, run the script using `node test.js`. You should see what in your code.

#### What Is Node.js Used For?
various build tools — designed to automate the process of developing a modern JavaScript application.

These build tools come in all shapes and sizes, and you won’t get far in a modern JavaScript landscape without bumping into them. They can be used for anything from bundling your JavaScript files and dependencies into static assets, to running tests, or automatic code linting and style checking.
And if you want to start developing apps with any modern JavaScript framework (for example, React or Angular), you’ll be expected to have a working knowledge of Node and npm (or maybe Yarn). This isn’t because you need a Node back end to run these frameworks. You don’t. Rather, it’s because these frameworks (and many, many related packages) are all available via npm and rely on Node to create a sensible development environment in which they can run.

#### The Node.js Execution Model
In very simplistic terms, when you connect to a traditional server, such as Apache, it will spawn a new thread to handle the request. In a language such as PHP or Ruby, any subsequent I/O operations (for example, interacting with a database) block the execution of your code until the operation has completed. That is, the server has to wait for the database lookup to complete before it can move on to processing the result

#### What Kind of Apps Is Node.js Suited To?
Node is particularly suited to building applications that require some form of real-time interaction or collaboration — for example, chat sites, or apps such as CodeShare, where you can watch a document being edited live by someone else.

#### What Are the Advantages of Node.js?
Aside from speed and scalability, an often-touted advantage of using JavaScript on a web server — as well as in the browser — is that your brain no longer needs to switch modes. You can do everything in the same language, which, as a developer, makes you more productive (and hopefully, happier). For example, you can easily share code between the server and the client.

Another of Node’s big pluses is that it speaks JSON. JSON is probably the most important data exchange format on the Web, and the lingua franca for interacting with object databases (such as MongoDB). JSON is ideally suited for consumption by a JavaScript program, meaning that when you’re working with Node, data can flow neatly between layers without the need for reformatting. You can have one syntax from browser to server to database.
#### Conclusion
JavaScript is everywhere, and Node is a vast and expansive subject. Nonetheless, I hope that in this article I’ve offered you the beginner-friendly, high-level look at Node.js and its main paradigms that I promised at the beginning. I also hope that when you re-read the definitions we looked at previously, things will make a lot more sense.