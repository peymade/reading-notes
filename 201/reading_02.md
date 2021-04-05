# Reading 2

## Duckett HTML

## Chapter 2: Text

Let's look at some of the building blocks of a webpage: the text! This list is a little cheat sheet for how to mark up text in HTML. 

* **Headings** can come in 6 different sizes. <h1> through <h6>. 
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

## Chapter 2: Basic JavaScript Instructions

## Chapter 4: Decisions and Loops


[Home](https://peymade.github.io/reading-notes/)