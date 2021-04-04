# Module 7 Reading 

## Pages 1-24 (Javascript)

### ABCs of Programming

Uses of JavaScript:
- Access Content ->  Content in the HTML, content inputted by users, etc.
- Modify Content -> Add & remove elements, attributes and text.
- Program Rules -> Create a set of rules that changes content on the page
- React to Events -> A specific script can run if parameters are met. Parameters can include: a link or button is clicked, specific information is inputted, or an amt of time has passed

### Approaching Programming

Programming can be looked at like a recipie, a manual, or a handbook. The computer will need the detailed, step by step instructions every single time there is a new problem to solve- and the code must be specific enough to account for every single step. 

1. Define the Goal  
Define the endpoints, the ideal solution of the puzzle
1. Design Script  
Break down the task into smaller sections, sometimes with a flowchart
1. Code the Steps  
Write out each step in a way the computer can interpret it


Flowcharts can be a great way to visually represent the different paths a computer program will take to complete the goal. 

## Pages 74-79 (JavaScript)

### Expressions

Two types of expressions:

1. Expressions that assign a value to a variable  
`var userName = 'Tom';`
1. Expressions that use multiple values to return one value  
`var area = 3 * 2`

### Operators

There are many types of operators. 

- Assignment operators = `userName = 'Tom';`
- Arithmetic operators = `area = 3*2;`
- String operators = `'Good ' + 'afternoon';`
- Comparison operators = `inventory = 3 > 9;` (false)
- Logical operators = `inventory = (3 > 9) && (8 < 3);` (false)

### Arithmetic Operators

When doing calculations, multiplication & division are prioritized. Use parentheses to avoid this. 

- Addition = +
- Subtraction = -
- Division = /
- Multiplication = *
- Increment = ++ (this adds 1 to the current number)
- Decrement = -- (this subtracts one from the current number)
- Modulus = % (this divides two values and returns the remainder)

### String Operator

The string operator is the + symbol. Adding strings together is called concatenation. 

When adding strings and numbers, the output will become a string. 
One can make numbers strings by placing '' around them. 

Example:

`var meal = 'Dinner ';`
`var thought = 'was good';`

`var mealStatment = meal + thought + '!';`


## Pages 88-94 (JavaScript)

Functions are helpful for grouping and storing code that can be reused in the future. 

Functions must be given individual names, and they can then be **called.** 
Pieces of information given to a function are **parameters.**
A function's response is a **return value.**

### Creating Functions

`function sayHello(){`
    `document.write('Hello!');`
`}`

`function` = Function Keyword
`sayHello()` = Function Name
`{document.write('Hello!');}` = Code block. Must be in curly braces.

### Calling Functions

To run the function, write the *function name* followed by parentheses.  
`sayHello();`

When the function has finished running, the code continues to run from where the function was called. 

### Declaring Functions with Parameters

Functions that need additional information have the parameters of that info placed in the parentheses after the function name. 

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

The `return` action will send a value out of the function and let it be shown on a webpage or used in other ways. 

**Example function:**

function calculateArea(width, height) {
    var area = width * height;
    return area;
}
var gardenOne = calculateArea(3, 5);
var gardenTwo = calculateArea(8, 8);

The function is being named "calculateArea" and the parameters are width and height. The function calculates the area, and returns this value. calculateArea then equals area. The variables of gardenOne and gardenTwo enter data for the parameters to use to calculate the area. 

[Home](https://peymade.github.io/reading-notes/)