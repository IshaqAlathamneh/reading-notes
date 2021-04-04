# Read-11

## EJS
What is the "E" for? "Embedded?" Could be. How about "Effective," "Elegant," or just "Easy"? EJS is a simple templating language that lets you generate HTML markup with plain JavaScript. No religiousness about how to organize things. No reinvention of iteration and control-flow. It's just plain JavaScript.

#### Some Features
* Fast compilation and rendering
* Simple template tags: <% %>
* Custom delimiters (e.g., use [? ?] instead of <% %>)
* Sub-template includes
* Ships with CLI
* Both server JS and browser support
* Static caching of intermediate JavaScript
* Static caching of templates
* Complies with the Express view system

#### How To istall EJS
It's easy to install EJS with NPM. just write:
`npm install ejs` in the terminal

#### EJS Tags

* `<% `'Scriptlet' tag, for control-flow, no output
* `<%_` ‘Whitespace Slurping’ Scriptlet tag, strips all whitespace before it
* `<%=` Outputs the value into the template (HTML escaped)
* `<%-` Outputs the unescaped value into the template
* `<%#` Comment tag, no execution, no output
* `<%%` Outputs a literal '<%'
* `%> `Plain ending tag
* `-%>` Trim-mode ('newline slurp') tag, trims following newline
* `_%>` ‘Whitespace Slurping’ ending tag, removes all whitespace after it

## Working with volumes
#### Performing a search
You can perform a volumes search by sending an `HTTP GET` request to the following URI:
`https://www.googleapis.com/books/v1/volumes?q=search+terms`

This request has a single required parameter:
* q - Search for volumes that contain this text string.  
special keywords for searching:

    * `intitle`: Returns results where the text following this keyword is found in the title.
    * `inauthor`: Returns results where the text following this keyword is found in the author.
    * `inpublisher`: Returns results where the text following this keyword is found in the publisher.
    * `subject`: Returns results where the text following this keyword is listed in the category list of the volume.
    * `isbn`: Returns results where the text following this keyword is the ISBN number.
    * `lccn`: Returns results where the text following this keyword is the Library of Congress Control Number.
    * `oclc`: Returns results where the text following this keyword is the Online Computer Library Center number.

Here is an example of searching for Daniel Keyes' "Flowers for Algernon":
`GET https://www.googleapis.com/books/v1/volumes?q=flowers+inauthor:keyes&key=yourAPIKey`

If the request succeeds, the server responds with a 200 OK HTTP status code and the volume results:
```
200 OK

{
 "kind": "books#volumes",
 "items": [
  {
   "kind": "books#volume",
   "id": "_ojXNuzgHRcC",
   "etag": "OTD2tB19qn4",
   "selfLink": "https://www.googleapis.com/books/v1/volumes/_ojXNuzgHRcC",
   "volumeInfo": {
    "title": "Flowers",
    "authors": [
     "Vijaya Khisty Bodach"
    ],
   ...
  },.....
  ```
* Filtering
You can use the filter parameter to restrict the returned results further by setting it the to one of the following values:

    * `partial` - Returns results where at least parts of the text are previewable.
    * `full` - Only returns results where all of the text is viewable.
    * `free`-ebooks - Only returns results that are free Google eBooks.
    * `paid`-ebooks - Only returns results that are Google eBooks with a price.
    * `ebooks` - Only returns results that are Google eBooks, paid or free. Examples of non-eBooks would be publisher content that is available in limited preview and not for sale, or magazines.

There's Also a lot of other parameters you can use and [read more about them](https://developers.google.com/books/docs/v1/using#WorkingVolumes).