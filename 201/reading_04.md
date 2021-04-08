# Reading 4

## Jon Duckett HTML Book

### Chapter 4- Links (74-93)

LINK EXAMPLES -->

* A basic link directing to external site: `<a href="http://wordpress.com">Wordpress</a>`
The text inside the opening tag includes the link, and the text that will display on the screen is enclosed in the element. 

* To link to other files with the relative link: `<a href="page2.html">About Us</a>`
The position of the file will have to be specified, if it is not in the same folder as the current file. For folders at higher levels, use the `../../index.html` way up moving up, and for folders at lower levels, specify their names `aboutus/careers/apply.html`

* To have a link that sends you to an email: `<a href="mailto:genericname@school.org">Email Owner of Site</a>`

* To have a link that opens in a new window: `<a href="http://www.wordpress.com" target="_blank">Wordpress</a> (new window)`

* To link to a part of a page: `<a href="#header">Take Me Back to the Top!</a>` 
This link would work if the header had an id tag of "header." This link is referring to that id tag, and would take you right back up to the top. If you are linking to a part of another page, place the url of that page before the id.

All these links work together to create a website. When a website has multiple pages, one could complete these steps:

1. Create a root folder, which stores the index.html for the main page
1. Create folders within the root folder for each page or category of pages
1. Make index.html file(s) in each folder

### Chapter 15- Layout (358-400)

We are going to dive into the core concepts of this chapter. 

CSS handles HTML elements either as blocks or inline elements. Block elements (`<p>, <ul>, <div>`) start on new lines, and inline elements (`<img>`) do not. Block level elements can sit inside other blocks, creating a direct parent relationship. 

With all of these following property and value combinations related to position, they can be accompanied by something like `left: 400px` which would then move the element, and other blocks would respond according to what value was assigned. 

### Normal Flow

* All block level elements stack on top of one another.
* `position: fixed`

### Relative Positioning

* Moving one element from it's normal spot in normal flow, while not affecting the blocks around it.
* `position: relative`
  
### Absolute Positioning

* The element is removed from the flow, and the space it leaves behind is filled in with the other elements.
  * `position: absolute`
* Fixed Positioning has something sit in relation to the browser window. This would be good if you had a heading that you wanted to stay visible as a user scrolled. 
  * `position: fixed`
* With Absolute positioning, you may need to use the z-index property. It controls the depth of elements. It is similar to the 'send to back' type language in design tools. The higher the number assigned to this index, the further front it will appear. 
  * `z-index: 10` is in front of `z-index: 2`

### Floating Elements

* This is similar to relative positioning, except in this case, other elements can be affected, and flow around it. 
* It places the affected element as far to the left or to the right as possible, in the containing element. 
* `float: left`

### Screen Size Challenges & Solutions

* A **fixed width layout** does not respond to changes in browser size
  * Measurments in pixels
  * Designer has greater control, at the cost of the site only working well on some screens
* A **liquid layout** responds to changes in browser size
 * Measurments in percentages
 * Tolerant of different font sizes, and leaves little white space on edges


## Jon Duckett JavaScript & JQuery Book

## Chapter 3 (pages 86-99)

Functions group and store code to be used multiple times.

Functions must be given names, and they can then be **called.**
Pieces of information given to a function (that it can then use in the function) are **parameters.**
A function's response is a **return value.**

### Creating Functions

`function sayGreeting(){`
    `document.write('Good Day!');`
`}`

`function` = Function Keyword
`sayGreeting()` = Function Name
`{document.write('Good Day!');}` = Code block. Must be in curly braces.

### Calling Functions

To run the function, write the *function name* followed by parentheses.  
`sayGreeting();`

When the function has finished running, the code continues to run from where the function was called.

### Declaring Functions with Parameters

Functions that need additional information have the parameters of that info placed in the parentheses after the function name. 

This example comes from page 92 of Duckett's JavaScript & JQuery book.

`function getArea(width, height){`
   `return width * height;`
`}`

`width` and `height` = Parameters

The above function both sets parameters, and then uses them like variables. 

### Calling Functions with Parameters

When calling a function with parameters, one must use arguments to specify what info will go in place of those parameters. 

- Arguments as Values = `getArea(3, 5);`
- Arguments as Variables = `wallWidth = 3;` `wallHeight = 5;` `getArea(wallWidth, wallHeight);`

### Getting a Value from a Function

The `return` action will send a value out of the function and let it be shown on a webpage or used in other ways. If you don't return some value, they can't be used outside the function.

**Example function:**

~~~
function calculateArea(width, height) {
    var area = width * height;
    return area;
}
var gardenOne = calculateArea(3, 5);
var gardenTwo = calculateArea(8, 8);
~~~

The function is being named "calculateArea" and the parameters are width and height. The function calculates the area, and returns this value. calculateArea then equals area. The variables of gardenOne and gardenTwo enter data for the parameters to use to calculate the area. 

[Home](https://peymade.github.io/reading-notes/)