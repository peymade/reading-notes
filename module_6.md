# Module 6 Reading

## Chapter 1 (Javascript Book)

### JavaScript foundations


html, css, and JavaScript all work together to create funcitoning web pages. 
- HTML is responsible for content
- CSS is responsible for the presentation of the content
- JavaScript handles how people interact with the site

By treating these three languages as layers, one can build a site with *progressive enhancement* in the order of HTML -> CSS -> JavaScript. 

It is important to try to keep everything in different files. One can use a single CSS sheet for a whole site, or make different ones. 

### Creating Basic JavaScript

- Keep separate folders to hold CSS, JavaScript, and HTML files 
- Use the .js ending when making a new JavaScript file
- Add links to .js files just before the closing </body> tag
- One can write JavaScript inside HTML files, but that is not best practice. Link the files together instead by using `<script src ="filename.js"></script>`
- To write the script directly in the HTML file, use the `<script></script>` tags directly in the code

### Objects & Methods

**`document.write('Good Afternoon!')`**

`document` = This is an object.  
`.` = This is a member operator. It is a way to access the members and properties within an object.  
`write` = This is a method. It allows some action to be taken.  
`'Good Afternoon'` = This is a parameter. THe write method needs some parameters to work, and it must be written in the parentheses. 

It matters where a script element is linked in the HTML, because that will determine where it shows up on the page. 

## Chapter 2 (Basic JavaScript Intructions)

### Statements

Statements are the individual intstructions given to the computer. This includes rules/guidelines being set, and commands being given. 

JavaScript is case sensitive. 
Each statement should end with a semicolon, and start on a new line. Also, multiple statements can be grouped together as a *code block* and wrapped in curly braces. 

### Comments

Add comments to script to explain what the code does. To make a section of script stop working temporarily, use a multi-line comment. 

- Multi-line = `/* Comment */`
- Single-line = `//`

### Variables

By setting variables, one can signal to the computer to remember some piece of information. 

The data stored in a variable can change, based on other variables, or user input, or other factors. 

`var quantity;`  
`var` = variable keyword. This indicates to the computer that one wants to create a variable  
`quantity` = variable name. This is the name/identifier of the variabe. 

Variables that are more than one word have the first word lower case and the second word capitalized. Like in `variableOne`

`quantity = 3;`  
In this example the equal sign is used as an *assignment operator.* This means that it sets the variable of "quantity" to the value of 3. 

### Data Types

One does not need to declare the type of data when creating a variable. 

- Numerical = Numbers. Fractions are written in decimal form, and there are no commas in large numbers. 
- String = Letters & other characters. Must be in single or double quotes. 
- Boolean = true or false. Like a lever or light switch- can help parts of the program run. 

### Other Notes on Variables

You can "escape" the quotation characters by adding a `\` in front of the first quotation mark and another `\` before the last. `\"sale.html\"`

Booleans can be for- 
- When a variable can only be (true/false) (on/off) (0/1)
- When code should split its path based on the outcome of a test

### Variable Naming

1. Begin with $, _, or letter. 
1. Do not include -, or . 
1. Do not use keywords.
1. Do not name different variables as same thing w/different capitalization.
1. Use semantic names.
1. Use camelCase.


## How Computers Work

- To be a computer, it must take input, store the inforamtion, process it, and output it. 
- Input devices take information from the physical world and convert it to binary
- Memory on a machine stores the information for later access
- A CPU, a central processing unit, calculated information
- Output is this binary information converted to a physical output

------

- Bit= The smallest piece of information a computer can store. When there are only two options, like on/off, yes/no, true/false, or 0/1. 
- All types of information can be stored in binary. More wires -> larger numbers
- Wires can feed into circuits that do simple calculations. When circuts are placed side by side, functionality increases.

------

- **CPU** = Master chip that controls the computer
- Circuits within the CPU perform basic math and logic, and store and share information
- Operating Systems control the software on a computer. When running multiple programs, the OS switches between them quickly. 




