# Reading 1

## Duckett HTML 

## Chapter 1: Structure & 17: HTML5 Layout

Structuring a HTML page is about creating hierarchies, and combining/layering elements. 

Elements are used to indicate the function of something on a web page. Elements are made up of tags. Some elements need just an opening tag, and some need both an opening and closing one. Here are some common ones and their functions:

* `<html></html>` This element indicates that the contents within it are written in HTML.
* `<body></body>` This element contains the code for things displayed on the page. Most things should go between these tags.
* `<head></head>` A place to store information or reference other files, like a CSS sheet.
* `<title></title>` The title of the page, shown at the top of the browser.

* `<h1></h1>` or `<h2></h2>` These elements are for heading text. These tags will affect the font size of text placed within it.
* `<p></p>` This element can contain the main content of a web page. Great for paragraphs. 
* `<article></article>` This element is great for content that can stand on its own. Article elements can be nested within other article elements. 
* `<header></header>` `<main></main>` and `<footer></footer>` These elements can help organize what informations is at the top, what is in the middle, and what is at the bottom of a webpage. 
* `<ul></ul>` The unordered list element is great for providing a list of links to other pages.
*`<li></li>` This element contains a list item.
* `<nav></nav>` A nav element indicates that the links will be used as a navigation bar.
* `<hgroup></hgroup>` This element is for grouping together multiple headings, so they are treated like one. 
* `<div></div>` This versatile element is used for grouping elements of all sorts. It is easy to add a class or id tag to it.

Elements can be given attributes and attribute values. 
`<img src="____">` 
In this example, src is the attribute name, and the value is in the quotation marks.

### A potential organization of basic elements on a web page made with HTML:

~~~

<!DOCTYPE html>
<html>
    <head>
        <title>TITLE</title>
    </head>
    <body>
        <header>
            <hgroup>
                <h1>Heading</h1>
                <h2>Sub-heading</h2>
            </hgroup>
            <nav>
                 <ul>
                     <li><a href="link">Link Name</a><li>
                     <li><a href="link">Link Name</a><li>
                     <li><a href="link">Link Name</a><li>
                 </ul>
             </nav>
        </header>

        <main>
            <section class="bold">
                <h3></h3>
                <p>TEXT</p>
            </section>
        </main>

        <footer>
        <p>TEXT</p>
        </footer>
    </body>
</html>
~~~

On page 445 of the book, there is great example HTML text. 

## Chapter 8: Extra Markup

Begin each HTML page with a DOCTYPE declaration: `<!DOCTYPE html>` 
To comment: `<!-- -->`

### id's and classes

Id's and classes are good ways to use attributes to distinguish and organize different elements on a page. 

Things to note:
* Only 1 item on each page can have a given id
* Multiple things can have the same class attribute
* Elements can have multiple classes associated with them, separated by a space
* Using `<div></div>` elements along with id's and classes can help by targeting grouping together elements that can later be modified by CSS as a group. These groupings will start on a new line.
* Use `<span></span>` along with id and class attributes to group together and style inline elements. 

## Chapter 18: Process & Design

How does one go about starting to design a website?
First, one has to ask some questions. For example:

* Who is the target audience?
* How familiar are they with websites? What are their goals? 
* Does my website provide entertainment or is it a tool to help them accomplish a task? 
* How do I present the information in a way relevant to *them*?

The answer to these questions helps build a **site map**

Site maps can be built using **card sorting**. 
* Place pieces of information on sheets of paper and organize them into related sections
* Organize it like the branches of a tree, and follow the logical hierarchies of information

**Wireframes** are page outlines without all the content. It can be good to present to a client before going and building the site. 

### Communicating the Message

* Be aware of all the content that must go on a web page. Be strategic with how you organize it, so it is not overwhelming.
* Make the key messages, terms, buttons, etc. look distinct. 
* Organize the content into related sections, to make it easier to digest.

**Size**, **color**, and **style** are helpful tools to make sure the reader finds the important information. 

Assume readers will be skimming each page. Help them find the important details. 
Be aware of keeping the pages and page elements consistent in their design, and organize the sections with headings. 

## Duckett JS

## Chapter 1: ABC of Programming

Let's define some of the vocabulary of JS!
* Objects = These are like any physical things. Inert on their own, but can be modified by events and properties.
* Properties = The characteristics of an object.
* Events = Interactions! These can be triggers for other things to happen in code.
* Methods = A way of updating things about the objects.

HTML, CSS, and JavaScript all work together to create funcitoning web pages. 
- HTML is responsible for content
- CSS is responsible for the presentation
- JavaScript is responsible for handling interactions and behavior

Each language is a layer. One can use *progressive enhancement* in the order of HTML -> CSS -> JavaScript. 

### Creating Basic JavaScript

- Keep separate folders to hold CSS, JavaScript, and HTML files 
- Use the .js ending when making a new JavaScript file
- Add links to .js files just before the closing </body> tag
- Do not write JavaScript inside HTML files. Link the files together instead by using a script tag with an src attribute --> `<script src ="filename.js"></script>`
- If you must write the script directly in the HTML file, use the `<script></script>` tags 

Let's look at an example of some JavaScript.

`document.write('Good Afternoon!')`

`document` = This is an **object**.  
`.` = This is a **member operator**. It is a way to access the members within an object.  
`write('Good Afternoon');` = This is a **method**. It allows action to be taken.  
`'Good Afternoon'` = This is a parameter. THe write method needs some parameters to work, and it must be written in the parentheses. 

Wherever the JavaScript is placed in the HTML, is where it will run. 

[Home](https://peymade.github.io/reading-notes/)