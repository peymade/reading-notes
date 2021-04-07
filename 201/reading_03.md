# Reading 3

## Jon Duckett HTML Book

Let's talk about **Lists!** (Chapter 3)

There are different types of lists. 
* Ordered Lists `<ol></ol>`
  * Outputs list items in 1. 2. 3. form
* Unordered Lists `<ul></ul>`
  * Outputs list items with something like bullet points
* Definition Lists `<dl></dl>`
  * `<dt></dt>` tags enclose *terms*  
  * `<dd></dd>` tags enclose *definitions*

Want to add an item to a list? Great! Put the item between these tags: `<li></li>`

Let's talk about **Boxes!** (Chapter 13)

The width and the height of boxes can be changed with percentages, so it reacts dynamically to the size of a browser/screen. 
The *min-width* and *max-width* properties can set limits on how large or small boxes can be stretched. The same goes for height, with *min-height* and *max-height*.

But what does one do if text gets cut off? You can decide what happens to it with the property *overflow*. Hidden --> Extra content not shown. Scroll --> Extra content included with scroll bar. 

Now, moving on to the space around the text. Directly around the text is the *padding*. Outside the box is the *margin*. And surrounding the box is the *border*. 

**Borders**: You can use the *border* property to declare width, type, and color (in that order) all at once! `border: 5px double black`
**Padding**: You can using the *padding* property to declare top, right, bottom, and left (in that order) all at once! `padding: 15px 5px 15px 5px`
**Margins**: You can use the same technique as padding above, or, you can use short hand to declare L&R and T&B in 2 numbers! `margin: 15px 20px`

**Centering a box** is a common need. Set the left-margin and right-margin to auto, and the text-align to center. Then it will be centered. 

Inline and block elements behave differently. You can switch one to behave like the other. Use the `display: inline` or `display: block` to achieve this. Use `display: inline-block` to have it keep some properties of block, while sitting like an inline. 

## Jon Duckett JavaScript & JQuery Book

Now, moving on to **Switch Statements!** (Chapter 4)
A switch statement checks a value against different cases. It can accomplish things similar to if/else statements. What differentiates it is how it checks against very specific cases. 

**Example Time!**

This example comes from a youtube video on freeCodeCamp.org's channel. The link: https://www.youtube.com/watch?v=fM5qnyasUYI

~~~
let day;
switch (new Date().getDay()){
 case 0:
    day = "Sunday";
      break;
  case 1:
  day = "Monday";
      break;
  case 2:
  day = "Tuesday";
      break;  
 case 3:
    day = "Wednesday";
      break;
  case 4:
  day = "Thursday";
      break;
  case 5:
  day = "Friday";
      break;  
 case 6:
    day = "Saturday";
      break;
}
~~~

The first line creates a variable of 'day.' The second line defines what condition is being checked- in this case, what day it is. If the number that is returned is 2, then the code beneath it will execute. In this case, that is assigning the string "Tuesday" to the variable "day." There is no default option in this case, because there will be no other output other than the listed options. 

Let's move on to **loops**!

3 main types of loops:
1. For
  * Run the code *for* a specific number of times. The condition can be a counter, with the loop including something like i++
1. While
  * These loops run until the condition becomes false. They can go on for a long time, if one is not careful. 
1. Do While
  * All statements are run, even if the condition is false. 

### Parts of a For Loop

The following 2 examples come from pages 170 and 176 in Jon Duckett's JavaScript & JQuery book.

~~~
for (var i = 0; i < 10; i++) {
    document.write(i);
}
~~~

- Initialization = `var i = 0;` This sets the counter to its starting point, and only happens once. 
- Condition = `i < 10;` This makes the condition true, until i reaches 10. 
- Update = `i++` This is doing the work of changing the value of i each time the loop repeats. 

### While Loops
~~~
var i = 1;
var msg = '';

while (i <10) {
    msg += i + ' x 5 = ' + (i *5) + '<br/>';
    i++;
}
~~~
This while loop checks the condition continuously, until i = 10, and then it stops printing out i * 5, and the value of that expression. 

[Home](https://peymade.github.io/reading-notes/)