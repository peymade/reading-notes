# Reading 9

## Jon Duckett's HTML Book

## Chapter 7- Forms (Pages 144-175)

Forms are great ways to get information from a user. They can come in the form of text input boxes, passowrds, comment boxes, radio buttons, checkboxes, drop down boxes, submit buttons, image buttons, and file uploads. 

A user presses the button, and their info is sent to and processed by a server. 

### Form Structure

Example form:
`<form action="url for page on server that receives the information" method="get or post"><p>Form Controls Appear Here</p>`
It must have the action attribute, and usually has method and id as well. 
The *get method* is for short forms or getting data from the web server. 
The *post method* is for long forms or sensitive information.

`<input>` is used to create different form controls. No closing tag. It is placed within the form element. 

- Example: `<input type="text" name="UserName" size="10" maxlength="25" />`
- The name indicates to the server what box of input this is
- maxLength limits the length of text input
- `type="password"` will automatically mask the characters, but does not handle the data securely

**Text Area** `<textarea></textarea>` is for multi-line text input. It has a closing tag- and between the opening and closing tags is the writing that automatically appears in the box. 

**Radio Buttons** let users pick multiple choice options. Example: `<input type="radio" name=genre" value="pop" checked="checked" />`

- The value does not appear on the screen- whatever is typed after this element is what appears on the screen.
- The checked attribute automatically checks this box when then page loads. 

**Checkboxes** let users select one or more options. Example: `<input type="checkbox" name="interests" value="reading" />`

**Drop-Down List Boxes** has users select one option from multiple. You must create a select tag and option values. You can turn it into a **Multiple Select Box** if you add a size attribute in the select tag. 


~~~
<select name="devices">
<option value="singing">Singing</option>
<option value="reading>Reading</option>
~~~

**File Input Boxes** let users upload files. Use the `type="file"` attribute in the input tag. 

**Submit Buttons** have the attribute `type="submit"` and send the data in the field to the server. 

### Other Noteds
- The button element can give you more control over apperance of buttons
- Use the `<label></label>` tag to enclose the input element to create a label for the box that will appear on the screen. Example: `<label>Greeting: <input type="text" name="greeting"/></label>`
- Group together fields with `<fieldset></fieldset>`
- The `<legend></legend>` element comes after fieldset, and is a title for what the group of fields is about. 
- Form validation is possible by adding the required attribute. 
- `type="date"` gathers date input in a more streamlined way
- `type="email" type="url"` can be used for emails and urls
- `type="search"` lets you enter a single search input

## Chapter 14- Lists, Tables, & Forms (pages 330-357)

### Lists

Use the `list-style-type` property to affect how lists look. 
- unordered lists can have bullet points, squares, circles...
- ordered lists can have roman numerals, letters, or numbers...

The `list-style-image: url('url')` property can be followed by a url, and will make the bullet points the specified image. 

The `list-style-position` can take *outside* and *inside* values to help move markers away from or towards the list content. 

The `list-style` property can help you list multiple of these at once. 

### Tables

Ideas for styling tables:

- Give cells padding
- Distinguish headers by making them bold
- Shade alternate rows (could be done by saying `tr.even {background-color:blue`)
- Use text align to align all numbers

- `border-spacing` lets you put space between the cells
- `border-collapse` pushes the cells together

### Forms

Notes on styling forms:

- Sometimes the boxes are not aligned. Set them to a specific width, and float the titles to the left. For the example, go to page 347
- Change the cursor stype when someone hovers over something
  - `cursor: pointer` or, auto, crosshair, default, move, text, wait, help. 

## Chapter 6- Events (pages 243-292)

Events indicate that something has happened. They can respond to something the user does, or to something like a web page loading.

- Events *fire* or are *raised* and they *trigger* script. 
- Three steps to doing event handling
  - Select the element that will be interacted with using DOM
  - Indicate the event on that node that triggers the script
  - Write the script that will be triggered
- `element.onevent = functionName;` This is the traditional DOM event handler
- Event listeners also work, but only in newer browsers. They can handle multiple functions
- Deault type of event flow is most specific -> least or *event bubbling*
- Attatch an event listener to a parent element, that will increase efficiency of code 
- The event object can tell you where the cursor was when it was clicked
  - Helpful for projects like the creation of a star on the click & location of the click
- There are keyboard events, mouse events, click events, form events, mutation events
  - Mutation events would be for when there is a change to the DOM

[Home](https://peymade.github.io/reading-notes/)