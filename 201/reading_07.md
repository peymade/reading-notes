# Reading 7

## Domain Modeling

Domain Modeling is creating a model in code for a specific goal. It can be a helpful tool in communicating the problem domain to various people involved. 

- Use the 'new' keyword to use a constructor function. 
- Use constructor functions to make things more efficient
- The constructor function creates properties inside an object using 'this'
- When multiple objects need to use the same function, you can set the function outside of the objects and add it to the constructor function's prototype. This means it can be used multiple times, instead of having the same method living in multiple objects. 

## Jon Duckett HTML Book- Chapter 6: Tables (126-145)

Creating a table

1. Use the  `<table></table>` element
1. Start a row with the `<tr></tr>` tag. 
1. Within the `<tr>` tags, place `<td></td>` tags 
1. Use the `<th scope="row or column"></th>` to add a heading to either a column or a row. Place it inside of a tr tag. like it is a row with an empty first item. Or place it above td elements in a row. 
1. Use the *colspan* or *rowspan* attributes to indicate an element should span more than one column. 
1. The elements within a table have scaffolding and structure. Separate the pieces with:
    - `<thead></thead>` contains the headings of the table
    - `<tbody></tbody>` contains the bulk of the data
    - `<tfoot></tfoot>` contains the footer of the table

## Jon Duckett JavaScript & JQuery Book- Chapter 3: Functions, Methods and Objects (106-144)

### Constructor Notation

Let's add some things to a new object, using dot notation. 
First, create the object. 
`var hotel = new Object();`
Then, add some properties using dot notation. 

~~~
hotel.name = 'Hyatt`
hotel.rooms = 50;
hotel.booked = 30;
hotel.checkAvailability = function(){
  return this.rooms - this.booked;
}
~~~

You can then update these properties simply by referring to the elements within the object like this: `hotel.name = 'New Name'`
You could also delete it: `delete hotel.name` or clear the value: `hotel.name = '';`

You can also use constructor notation to create multiple objects using one function. Like this: 

~~~
function Hotel(name, rooms, booked) {
  this.name = name;
  this.rooms = rooms;
  this.booked = booked;

  this.checkAvailability = function() {
    return this.rooms - this.booked;
  };
}
~~~ 

What this block of code does, is it takes in 3 parameters: the name of the hotel, the total rooms, and the number of them booked. It then creates an object based on this data. In order to *use* the function above, we do this: `var seasonsHotel = new Hotel('Seasons', 500, 300);`
That can be repeated multiple times, and each time a new object will be created. 

If you wanted to display the output of the function within the Hotel object on the webpage, you could access it like this: `var elementRooms = document.getElementById('rooms'); elementRooms.textContent = hotel.checkAvailability();`

So in summary- you can either create the object first, then add properties and methods to it, or you can create it with all of that already attatched, by using literal notation or a function. 

### Ways to Store Data

- Variables
  - One key and one value
- Arrays
  - Data whose order matters should be in an array
  - Arrays are a special type of object. You can have either one contain the other. An array full of objects or an object full of arrays. 
- Individually crafted Objects
  - There are multiple keys in an object
- Multiple objects 
  - Multiple objects can be generated with a function

### Built in Objects

Browsers come with built-in objects that represent the browser window and other things. 
An **object model** is a group of objects that form some larger thing. 

The **Browser Object Model** contants objects pertaining to the current browser or tab. Window -> Document ->History -> Location -> Navigator -> Screen, and so on. You could use `window.screen.width` to see the device screen width. Helpful!

The **Document Object Model** contains objects that create a representation of the current page. The child elements all stem from the document object. You could use `document.lastModified` to see which element was last changed. 

**Global JavaScript Objects** live within the JavaScript language, and can perform helpful tasks to do with things like dates and math. You could use `Math.PI();` to list the digits of pi. So cool. 

### Global Objects

- All strings have index numbers to represent the characters. These values can be accessed and with global objects like saying: `stringName.charAt(19);`
- Some number objects (the last 3 return strings)
  - `isNaN()` checks if the value is not a number
  - `toFixed()` rounds the number to inputted number of decimal points
  - `toPrecision()` rounds to total inputted number given
  - `toExponential()`gives the number in exponential notation 
- Math objects 
  - `Math.PI` returns pi
  - `Math.round()` rounds to nearest integer
  - `math.sqrt(number)` returns square root
  - `Math.ceil()` rounds to nearest integer
  - `Math.floor()` rounds number down to integer
  - `Math.random()` generates a random number between 0 and 1
  - Creating random numbers: `var random = Math.floor((Math.random() * 10) + 1);`
- Date Objects
  - `var today = new Date();` After creating the date object, you can access it and set the time and date. See page 137 for a full list of these objects. 
  




[Home](https://peymade.github.io/reading-notes/)