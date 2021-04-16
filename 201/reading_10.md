# Reading 10

## Jon Duckett Chapter 10- Error Handling & Debugging

Every statement lives in one of three contexts. The context determines the scope of things inside it. Variables created in a function are limited to that function, unless returned or sent out. 

- GLobal context- in the script, but not in function
- Function context- in a function
- Eval Context

- When a function is called, the code immediately goes to that function and runs it, before continuing with the rest of the code. 
- You can call functions or alter variables before they are formally made in the script, because the preparation of these things, and their creation, happens before other things in the script. 
- Use the developer tool to give clues as to where the code broke. It will often give a line number, and a message as to why the code stopped. 
- Enter in the error to google- because it could mean something very specific and fixable. 

### Breakpoints

Set a breakpoint to see what the variables are at a certain point in your code. You can use breakpoints to move through the code to identify issue spots. Also use console.logs. 

1. Select *sources* in the Chrome developer tools
1. Select the script you are working on
1. Find the line number and click on it
1. Right click to add a condition (optional)

### Debugging Tips

- Open live server in a different browser
- Comment out parts of the code
- Open a new JS file and alter the code in more drastic ways without deleting the old stuff
- Explain the code to someone else
- Post on forums or search online
- Beware of common errors:  
  - Capitalization. JavaScript is case sensitive. 
  - Issues with variable scope- trying to access a variable that is in a function and not being sent out. 
  - Missing semicolons and ending brackets
  - === versus == versus =. 
  - Check script for missing parameters for functions




[Home](https://peymade.github.io/reading-notes/)