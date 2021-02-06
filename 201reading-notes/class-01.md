# Class-01
summrize the first class

 ##  How the Web Works
 When you visit a website, the web server hosting that site could be anywhere in the world. In order for you to find the location of the web server, your browser will first connect to a Domain Name System (DNS) server.
## HTML Uses Elements to Describe the Structure of Pages
Tags act like containers. They tell you something about the information that lies between their opening and closing tags.
## Attributes Tell Us More About Elements
Attributes provide additional information about the contents of an element. They appear on the opening tag of the element and are made up of two parts: a name and a value, separated by an equals sign.
## Summary Structure 
* HTML pages are text documents.
* HTML uses tags to give the information they surround special meaning.
* Tags are often referred to as elements.
* Tags usually come in pairs. The opening tag denotes the start of a piece of content; the closing tag denotes the end.
* Opening tags can carry attributes, which tell us more about the content of that element.
* Attributes require a name and a value.
* To learn HTML you need to know what tags are available for you to use, what they do, and where they can go.
## Extra Markup
* DOCTYPE 
Because there have been several versions of HTML, each web page should begin with a DOCTYPE declaration to tell a browser which version of HTML the page is using.
* Comments in HTML
If you want to add a comment to your code that will not be visible in the user's browser, you can add the text between these characters:
<!-- comment goes here -->
* ID Attribute
Every HTML element can carry the id attribute. It is used to uniquely identify that element from other elements on the page.
* Class Attribute
Every HTML element can also carry a class attribute. Sometimes, rather than uniquely identifying one element within a document, you will want a way to identify several elements as being different from the other elements on the page.
* Block Elements
Some elements will always appear to start on a new line in the browser window.
* Inline Elements
Some elements will always appear to continue on the same line as their neighbouring elements.
* Grouping Text & Elements In a Block
The <div> element allows you to group a set of elements together in one block-level box.
* Grouping Text & Elements Inline
The <span> element acts like an inline equivalent of the <div> element. It is used to either:
1. Contain a section of text where there is no other suitable element to differentiate it from its surrounding text
1. Contain a number of inline elements
* IFrames
* Information About Your Pages
The <meta> element lives inside the <head> element and contains information about that web page.
## Escape Characters
There are some characters that are used in and reserved by HTML code.
![chaeacters](sym.jfif)
## HTML5 Layout
* The new HTML5 elements indicate the purpose of different parts of a web page and help to describe its structure.
* The new elements provide clearer code (compared with using multiple <div> elements).
* Older browsers that do not understand HTML5 elements need to be told which elements are block-level elements.
* To make HTML5 elements work in Internet Explorer 8 (and older versions of IE), extra JavaScript is needed, which is available free from Google.
## Process & Design
* It's important to understand who your target audience is, why they would come to your site, what information they want to find and when they are likely to return.
* Site maps allow you to plan the structure of a site.
* Wireframes allow you to organize the information that will need to go on each page.
* Design is about communication. Visual hierarchy helps visitors understand what you are trying to tell them.
* You can differentiate between pieces of information using size, color, and style.
* You can use grouping and similarity to help simplify the information you present.
## The ABC of programming

### A: what is a script and how do I creat one?
* A script is a series of instructions that the computer can follow in order to achieve a goal. 
* Each time the script runs, it might only use a subset of all the instructions. 
* Computers approach tasks in a different way than humans, so your instructions must let the computer solve the task prggrammatically.
* To approach writing a script, break down your goal into a series of tasks and then work out each step needed to complete that task (a flowchart can help). 
### B: How do computers fit in with the world around them?
* Computers create models of the world using data
* The models use abjects to represant physical things Obectcan hae properties that tell us about the object methads that perform tasks using the DrOperties of that ob ect events which are triggered when a userinteracts with the computer.
* Programmers can write cade to say When this event occurs run that code.
* Web browsers use HEM markupito create a model of the web paga kah element areatos its own nade (which is a kind ol ogeat).
* To make web pages interactivs you write code that uses the browser's model of the web page.



### C: how do I write a script for a web page?
* It is best to keep JavaScript code in its own JavaScript file. JavaScript files are text files (like HTML pages and CSS style sheets), but they have the . j s extension.
* The HTML <script> element is used in HTML pages to tell the browser to load the JavaScript file (rather like the <link> element can be used to load a CSS file). 
* If you view the source code of the page in the browser, the JavaScript will not have changed the HTML, because the script works with the model of the web page that the browser has created. 