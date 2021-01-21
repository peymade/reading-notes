# Module 5 Reading

## Chapter 10: Introducing CSS

### How to use CSS

CSS rules can be applied to different elements built with HTML. Boxes created with `<h1> <p>` and such can be modified with regards to the border color, text size, fill color, and many other specifications. 

### Parts of CSS Specification

`p { font-family: Arial;}`

The part outside the brackets is a selector, the part inside is the declaration. This rule says that all `<p>` elements should be shown in Arial font. 

Declarations are made of a property and a value. 

Go to page 238 in the textbook for a chart on different selectors. 

## Chapter 11: Color

### Foreground

Three ways to specify color for text:

- RGB Values: `rgb(100,99,78)`
- Hex Codes: `#ee8e90`
- Color Names: `DarkCyan`

For all these options, the selector is the element whose text will take on these changes, and the property is `color`

### Background

To make sure that the browser background color is consistent, always set it to something. If that color is white, set `<body>` to white. 

### Contrast

Text must be readable, so contrast is a must. Low contrast is something to avoid- High contrast mixed with medium contrast is a good way to achieve balance.  

### Opacity

To add opacity, one can use the rgba property instead of just rgb. The a represents opacity- and must be a value between 0.0 and 1.0.  
Or, simply use the property `opacity` and set the value. 

### hsla

By adding the letters `hsla` or `hsl` before a set of numbers following the background color property, one can control even more aspects of color.  
1. H = Hue = a degree between 0 and 360
1. S = Saturation = a percent between 0% and 100% (0 is gray, 100 is full color)
1. L = Lightness = a percent between 0% and 100% (0 is white, 100 is black)
1. A = Opacity = a number between 0 and 1.0 (0 is transparent, 100 is solid)

