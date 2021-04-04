# Module 8 Reading

## Pages 150-151, 156, 157, 170-173, 176 (Javascript)

### Comparison Operators (150 & 151)

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

### Logical Operators (156 & 157)

Logical operators look at multiple comparison statements, and evaluate the results of them together. 

`((5 < 2) && (2 .= 3))`

In this example, the double ampersands are asking the question: "do both the comparison operator statements result in *true*? Since the answer is no, the expression as a whole evaluates to false. 

- `&&` Logical And. If both expressions are true, this is true. If any one of them or both of them is false, it evaluates to false. 
- `||` Logical Or. If either expression is true, this returns true. 
- `!` Logical Not. This reverses a boolean. If the value was false, when one does `!(2 < 1)` and it becomes true. 

### Loops (170-173)

Loops check conditions, and if the condition evaluated to true, the code runs and repeats until the condition is false. 

- For Loops = for running a code a specific number of times
- While Loops = for running code an unknown number of times
- Do While Loops = for running code at least once even if the condition is false

### Parts of a For Loop

`for (var i = 0; i < 10; i++) {`
   ` document.write(i);`
`}`

- Initialization = `var i = 0;` This sets the counter to its starting point, and only happens once. 
- Condition = `i < 10;` This makes the condition true, until i reaches a certain number. 
- Update = `i++` This is doing the work of changing the value of i each time the loop repeats. 

### While Loops

`var i = 1;`
`var msg = '';`

`while (i <10) {`
  `  msg += i + ' x 5 = ' + (i *5) + '<br/>';`
   ` i++;`
`}`

This while loop checks the condition continuously, until i = 10, and then it stops printing out i * 5, and the value of that expression. 

[Home](README.md)
