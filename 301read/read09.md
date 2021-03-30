# Read-09

### Concepts of Functional Programming in Javascript
***Complexity*** is anything that makes software hard to understand or to modify.

***What is functional programming?***
Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data 

how do we know if a ***function is pure*** or not? Here is a very strict definition of purity:
* It returns the same result if given the same arguments
* It does not cause any observable side effects

#### Immutability
*Unchanging over time or unable to be changed.*
When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

#### Referential transparency
Passing 2 as a parameter of the square function will always returns 4. So now we can replace the square(2) with 4. That's it! Our function is referentially transparent.
**pure functions + immutable data = referential transparency**

#### Functions as first-class entities
The idea of functions as first-class entities is that functions are also treated as values and used as data.
Functions as first-class entities can:
* pass it as a parameter to other functions 
* refer to it from constants and variables
* return it as result from other functions
The idea is to treat functions as values and pass functions like data. This way we can combine different functions to create new functions with new behavior.
#### Higher-order functions
When we talk about higher-order functions, we mean a function that either:
* takes one or more functions as arguments, or
* returns a function as its result
#### Array's methods
* Filter: Given a collection, we want to filter by an attribute. The filter function expects a true or false value to determine if the element should or should not be included in the result collection.
* Map: The map method transforms a collection by applying a function to all of its elements and building a new collection from the returned values.
* Reduce: The idea of reduce is to receive a function and a collection, and return a value created by combining the items.
#### Strategies
Here are some straightforward to implement methods that can lead to easier to read code. There are no absolutes when it comes to clean code — there's always an edge case!
* Return early from functions:
```
function showProfile(user) {
  if (user.authenticated === true) {
    // ..
  }
}

// Refactor into ->

function showProfile(user) {
  // People often inline such checks
  if (user.authenticated === false) { return; }
  // Stay at the function indentation level, plus less brackets
}
```
* Cache variables so functions can be read like sentences:
```
function searchGroups(name) {
  for (let i = 0; i < continents.length; i++) {
    for (let j = 0; j < continents[i].length; j++) {
      for (let k = 0; k < continents[i][j].tags.length; k++) {
        if (continents[i][j].tags[k] === name) {
          return continents[i][j].id;
        }
      }
    }
  }
}

// Refactor into ->

function searchGroups(name) {
  for (let i = 0; i < continents.length; i++) {
    const group = continents[i]; // This code becomes self-documenting
    for (let j = 0; j < group.length; j++) {
      const tags = group[j].tags;
      for (let k = 0; k < tags.length; k++) {
        if (tags[k] === name) {
          return group[j].id; // The core of this nasty loop is clearer to read
        }
      }
    }
  }
}
```
* Check for Web APIs before implementing your own functionality:
```
function cacheBust(url) {
  return url.includes('?') === true ?
    `${url}&time=${Date.now()}` :
    `${url}?time=${Date.now()}`
}

// Refactor into ->

function cacheBust(url) {
  // This throws an error on invalid URL which stops undefined behaviour
  const urlObj = new URL(url);
  urlObj.searchParams.append('time', Date.now); // Easier to skim read
  return url.toString();
}
```
It's important to get your code right the first time because in many businesses there isn't much value in refactoring.
### Resources
* [medium](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)
* [dev](https://dev.to/healeycodes/refactoring-javascript-for-performance-and-readability-with-examples-1hec)