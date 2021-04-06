# Reading 2

## Duckett HTML

## Chapter 2: Text

Let's look at some of the building blocks of a webpage: the text! This list is a little cheat sheet for how to mark up text in HTML. 

* **Headings** can come in 6 different sizes. `<h1>` through `<h6>`. 
* **Paragraphs** will always show on a new line. Use the <p> tag.
* **Bold & Italic** can be created using `<b></b>` tags and `<i></i>` tags.
* **Superscript and Subscript** can be created by enclosing the desired changed text in `<sup></sup>` or `<sub></sub>` tags.
* **Line Breaks** can be placed using the `<br />` tag at the desired break. This is a single tag element.
* **Horizontal Lines** can be added by using the `<hr />` tag.
* **Strong and Emphasis** tags, `<strong></strong>` and `<em></em>` can enclose text to make it either bold or italics. 
* **Quotations** can be made using a `<blockquote></blockquote>` or a `<q></q>` element. The blockquote tags are more for larger quotes, and the q tags are for quotes within text.
* **Changes** can be indicated using the `<ins></ins>` and `<del></del>` elements, which will add underlines and strikes to most enclosed text, or an `<s></s>` tag, that is for outdated information that should still be displayed.
* **Citations and Definitions** are indicated using `<cite></cite>` and `<dfn></dfn>` tags. Cite will make things italic, and dfn will not change the text.

## Chapter 10: Introducing CSS

CSS rules can be applied to different elements built with HTML. Items created with either block or inline elements can be modified with regards to the border color, text size, fill color, and many other specifications. 

### Parts of CSS Specification 

This example comes from page 231 of Duckett's HTML book. 

~~~
p { 
    font-family: Arial;}
~~~
The part outside the brackets is a selector, the part inside is the declaration. This rule says that all `<p>` elements should be shown in Arial font. 

Declarations are made of a property and a value. In this case, the property is the font, and the value is which font it is: Arial. 

Page 238 in Duckett's HTML book has a chart on different selectors. 4 common selectors:

* `* {}` Is for all elements on a page
* `.class {}` Is for all elements of a certain class
* `#id {}` Is for the element matching an id
* `h1, h2, h3 {}` Is for all items that match the listed elements. Could also be `p, a, h1 {}`

### How do "Cascading Style Sheets" Cascade?

The last selector will take precedence over an earlier, identical one. A more specific selector will take precedence over a more general one. And a value with `!important` added after it will take precedence. 

## Duckett JavaScript & JQuery
## Chapter 2: Basic JavaScript Instructions

JavaScript basics! Let's start with building blocks. Those are **statements**. Statements are the individual intstructions given to the computer. If a program is a manual for setting up a piece of furniture, statements are the basic steps. They can be definitions of what different parts are, etc. 

Adding **comments** to script is like writing notes in the margins of this 'manual.' Notes can explain what the code does to others, or to a future self. You can also comment out a section of script to make it stop working temporarily. 

* Multi-line = `/* Comment */`
* Single-line = `//`

**Variables** are placeholders for information.
The data stored in a variable can change based on the status of/data stored in another variable, or can change based on user input. 

**Example Time!**

`var amtPaid;`  
`var` = This variable keyword signals to the computer that you wants to create a variable  
`amtPaid` = This variable name is the bucket/bin. It is the storage unit that holds the information and can be recalled.

`amtPaid = 10;`  
The equal sign here is being used as an *assignment operator.* This operator has set the variable of "amtPaid" to the value of 10. 

Unlike in some other languages, one does not need to declare the type of data when creating a variable. 

* Numeric = Numbers 
    * Fractions are written in decimal form, and there are no commas in large numbers. 
* String = Letters & other characters 
    * Must be in single or double quotes. 
* Boolean = true or false 
    * Like a lever or light switch- helps a program split a path on the outcome of a test. (true/false) (on/off) (0/1) 

### Rules for Variable Naming

1. Begin with $, _, or letter. 
1. Do not include -, or . 
1. Do not use keywords.
1. Do not name different variables as same thing w/different capitalization.
1. Use semantic names.
1. Use camelCase.
1. You can "escape" characters by adding a slash `\` in front of each special character. `\"quotation\"`

*^These rules directly from Jon Duckett's JavaScript and JQuery book, on page 69.*

### Arrays

* Arrays store multiple pieces of information in a list, that are related to each other. 
* Arrays start in the '0' position!


**Example Time!** 
~~~
var food;
food = ['banana', 'sandwich', 'butter'];

var foodTwo
foodTwo = food[1]

var totalFood
totalFood = food.length;

food[1] = 'ham';
~~~

This code assigns an array to three values, then selects the second one, and sets another variable equal to the length of the array. Then, it reassigns the second position to a different term: ham.

**Updating Variables** 
`var faveFood = 'cheese';`
To change this from cheese to bread, I do this:
~~~
var elFaveFood = document.getElementbyId('faveFood');
elFaveFood.textContent = bread;
~~~

### Expressions and Operators

Expressions can--
* Assign values to variables --> `var food = 'lemon';`
* Use multiple values to calculate/make a variable --> `var avgSpeed = 10/200`

**Operators** are ways to combine values. 
* Assignment Operators --> food = 'banana';
* Arithmetic Operators --> avgSpeed = 10/200;
    * Addition (+) Subtraction (-) Division (/) Multiplication (*) Add 1 to current number (++) Subtract 1 from current number (--) Divide and return remainder (%)
* String Operators --> name = 'Jane ' + 'Thomas';
    * Only use the (+) 
* Comparison Operators --> wins = 9 < 3; (false)
* Logical Operators --> wins = (8>4) && (5<10); (true)

## Chapter 4: Decisions and Loops

### Comparison Operators

These are all used to **evaluate conditions**. 

- `==` is equal to. This returns "true" if two values are the same. 
- `!=` is not equal to. This returns "true" if two values are not the same. 
- `===` is strict equal to. This returns "true" if both values are the same AND the data type is the same. 
- `!==` is strict not equal to. This returns "true" if both the value AND the data type are different. 
- `>` Greater than
- `<` Less than
- `>=` Greater than or equal to
- `<=` Less than or equal to

These operators all return either a **true** or a **false** output. 

### Logical Operators 

Logical operators look at multiple comparison statements, and evaluate the results of them together. 

`((5 < 2) && (2 .= 3))`

In this example, the double ampersands are asking the question: "do both the comparison operator statements result in *true*? Since the answer is no, the expression as a whole evaluates to false. 

- `&&` Logical And. If both expressions are true, this is true. If any one of them or both of them is false, it evaluates to false. 
- `||` Logical Or. If either expression is true, this returns true. 
- `!` Logical Not. This reverses a boolean. If the value was false, when one does `!(2 < 1)` and it becomes true. 

### If Statements

If statements help to check conditions and execute (or not execute) code based on the results. The if statement below triggers the running of the subsequent code, which sets the output variable equal to a string.

Adding an 'else' to an if statement adds code to execute if the expression is false. 

**Example Time!**
~~~
var runLength = 20;
var output;
if (runLength >= 10) {
    output = 'Wow, that's a long way to run.';
}
~~~



[Home](https://peymade.github.io/reading-notes/)