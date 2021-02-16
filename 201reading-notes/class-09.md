# Read-09

## forms
Why Forms? The best known form on the web is probably the search box that sits right in the middle of Google's homepage

***Form Controls:*** There are several types of form controls that you can use to collect information from visitors to your site.
1. ADDING TEXT: Text input , Password input , Text area.
1. Making Choices: Radio buttons, Checkboxes, Drop-down boxes.
1. Submitting Forms: Submit buttons, Image buttons, File upload

***How Forms Work***

* A user fills in a form and then presses a button to submit the information to the server.
* A form may have several form controls, each gathering different information. The server needs to know which piece of inputted data corresponds with which form element.
* Information from a form is sent in name/value pairs
* HTML5 introduces new form elements which make it easier for visitors to fill in forms.

## Lists, Tables and Forms
There are several CSS properties that were created to work with specific types of HTML elements, such as lists, tables, and forms.

***Styling Forms***

CSS is commonly used to control the appearance of form elements. This is both to make them more attractive and to make them more consistent across different browsers.

* Styling Fieldsets & Legends: The legend is used to indicate what information is required in the fieldset.
* Cursor Styles: The cursor property allows you to control the type of mouse cursor that should be displayed to users.

***Web Developer Toolbar***

This helpful extension for Firefox and Chrome provides tools to show you the CSS styles that apply to an element when you hover over it, along with the structure of the HTML.

***Summary***

* List markers can be given different appearances using the list-style-type and list-style image properties.
* Table cells can have different borders and spacing in different browsers, but there are properties you can use to control them and make them more consistent. 
* Forms benefit from styles that make them feel more interactive.
## Events
When you browse the web, your browser registers different types of events. It's the browser's way of saying, "Hey, this just happened." Your script can then respond to these events. 
- ***INTERACTIONS CREATE EVENTS:***
Events occur when users click or tap on a link, hover or swipe over an element, t ype on the keyboard resize the window, or when the page they requested has loaded.
- ***EVENTS TRIGGER CODE***
When an event occurs, or fires, it can be used to trigger a particular function. Different code can be triggered when users interact with different parts of the page.
- ***CODE RESPONDS TO USERS***
In the last chapter, you saw how the DOM can be used to update a page. The events can trigger the kinds of changes the DOM is capable of. This is how a web page reacts to users.
 ### Summary 
 * Events are the browser's way of indicating when something has happened (such as when a page has finished loading or a button has been clicked). 
 * Binding is the process of stating which event you are waiting to happen, and which element you are waiting for that event to happen upon. 
* When an event occurs on an element, it can trigger a JavaScript function. When this function then changes the web page in some way, it feels interactive because it has responded to the user.
* You can use event delegation to monitor for events that happen on all of the children of an element. 
* The most commonly used events are W3C DOM events, although there are others in the HTMLS specification as well as browser-specific events.