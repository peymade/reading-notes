# Module 4 Reading

## Chapter 18: Process & Design

### Who is the site for?

Identify the target audience. 
* What are their goals? How familiar are they with websites?
* Does my website provide entertainment or is it a tool to help them accomplish a task? 

All in service of this question:
* How do I present the information in a way relevant to *them*?

The answer to these questions helps build a **site map**

Site maps can be build using **card sorting**. 
* Place pieces of information on sheets of paper and organize them into related sections
* Organize it like the branches of a tree
* Start with "HOME" at top, then primary nav links

**Wireframes** are page outlines without all the content. It can be good to present to a client before going and building the site. 

### Communicating a Message

Content, Prioritize, Organize. 

* Widdle down the content and make it clear and accesible to the target audience. 
* Prioritize the key messages, terms, buttons, etc.
* Organize the content into related sections, to make it easier to digest

**Size**, **color**, and **style** are also helpful tools to make sure the reader finds the important information. 

Assume readers will be skimming each page. Help them find the important details. 

## Chapter 17: HTML Layout

### HTML5

HTML5 has a few differences. For example instead of using div elements, HTML5 offers new names for different parts of a web page. Just to name a few-
* article
* nav
* aside

### Headers & Footers

`<header> and <footer>`

One can have a header & footer pairing for a section of a site, or for the whole site. 

A header/footer could be useful for a section by having the header be the title, and the footer being social media links.

### Navigation

`<nav>`

The nav element contains links for site navigation. Mainly primary navigation, sometimes for links at the bottom of the page. 

### Articles

`<article>`

Each independent piece of written information lives inside of an article block. 

Articles can be nested, and each page can contain multiple. 

### Asides

`<aside>`

An aside inside of an article contains information not essential to the content of the article. Outside, and it stores information relevant to the entire page. 

### Sections

`<section>`

This element groups content together. 
Each usually has its own heading.

The article elements can be nested inside one section element, or vice versa. Section is not good for being the element wrapping the text of the entire page. That is a job for `<div>`

### Heading Groups 

`<hgroup>`

This element groups different sized headers together, usually a heading and a subtitle. 

### Figures

`<figure>`

This element is for content that the essential text refrences, for example an image, video, graph, diagram, or code sample. One adds a `<figcaption>` to go along with the content. 

### Sectioning Elements

`<div>`

The div element is used to group together elements, especially when the other above elements won't do the job.

### Linking Block Level

`<a>`

One can use the a element to link a whole block that contains child elements. 


### Older Browswers

To help older browsers recognize the new elements, add these things:

**CSS**  
`header, section, footer, aside, nav, article, figure {display:block;}`  
**HTML**
`<!--[if lt IE 9]> <script src="http://html5shiv.googlecode.com/svn/trunk/html5.js"></script><![endif]-->`

## Chapter 8: Extra Markup


Begin each webpage with a **DOCTYPE** declaration: `<!DOCTYPE html>`

**Comment format**: `<!-- COMMENT -->

**ID Attribute**: place `id=""` at the end of the element opening bracket. It must begin with a letter or an underscore
This attribute can be used on any element. Helpful for styling purposes. 

**Class Attribute**: place `class=""` at the end of the element opening bracket. Things can have more than one class tag. 

**Block Elements**: elements like `<h1><p><ul> and <li>` all start on new lines automatically. 

**Inline Elements**: these elements do not automatically start on a new line. Things like `<a><b><em><img>`

**Div Elements**: This allows for grouping of different elements. You must give it an id with a name. This is useful for CSS styling. 

**Span**: Used to group inline elements to make styling easier. `<span>` There also must be a class or id assigned to it like with a div element. 

**iframe** A window into another webpage. Must have width and height specified, and a `src`

**Escape Characters** For multiple characters like quotation marks and angled brackets, different combinations of characters need to replace them. Look this up for a complete list. 

