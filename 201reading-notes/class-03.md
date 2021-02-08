# Class-03

## Lists
There's three types of list in html:
1. Ordered Lists: it's created with the `<ol>` element, each item in the list placed between `<li>` and `</li>`.
1. Unordered Lists: it's created with the `<ul>` element, each item in the list placed between `<li>` and `</li>`.
1. Definition Lists: it's created with the `<dl>` element, `<dt>`This is used to contain the term being defined, `<dd>` This is used to contain the definition.
1. Nested Lists: You can put a second list inside an `<li>` element to create a sublist or nested list.

## Boxes
At the beginning of this section on CSS, you saw how CSS treats each HTML element as if it lives in its own box.
* Box Dimensions: like width and hight.
* Limiting Width: min-width, max-width.
* Limiting Height: min-height, max-height.
* Overflowing Content: The overflow property tells the browser what to do if the content contained within a box is larger than the box itself. It can have one of two values: 
    1. hidden
    1. scroll

***Border, Margin & Padding:*** 
Every box has three available properties that can be adjusted to control its appearance:
1. Border: Every box has a border (even if it is not visible or is specified to be 0 pixels wide). The border separates the edge of one box from another.
1. Margin: Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes.
1. Padding: Padding is the space between the border of a box and any content contained within it. Adding padding can increase the readability of its contents.

*The padding and margin properties are very helpful in adding space between various items on the page*
*If you want to center a box on the page , you can set the left-margin and right-margin to auto*
*The display property allows you to turn an inline element into a block-level element or vice versa, and can also be used to hide an element from the page*
*The visibility property allows you to hide boxes from users but It leaves a space where the element would have been.*
*Legibility can be improved by controlling the width of boxes containing text and the leading.*
*CSS3 has introduced the ability to create image borders and rounded borders*
### ARRAYS 
An array is a special type of variable. It doesn't just store one value; it stores a list of values. 
**You create an array and give it a name just like you would any other variable (using the var keyword followed by the name of the array).**
The values are assigned to the array inside a pair of square brackets, and each value is separated by a comma.
* VALUES IN ARRAYS 
Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one). 
**To access a value from an array, after the array name you specify the index number for that value inside square brackets**
## If else statments 
The if else statements check a condition if it's true the first code will run and if it's false the second code will run.
## SWITCH STATEMENTS 
A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that value.You have a default option that is run if none of the cases match.
switch statements allow you to compare a value against possible outcomes.

* Data types can be coerced from one type to another.
* All values evaluate to either truthy or falsy. 

## Loops:
1. For
1. While
1. Do While
