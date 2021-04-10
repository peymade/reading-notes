# Reading 5

## Quick note on Git Branching

1. navigate to the main repo in local terminal
1. `git checkout -b branchName`
1. `code .` on new branch, then move on to step 4 when done coding
1. `git add *`
1. `git commit -m "message"`
1. `git push origin branchName`
1. go to github and create pull request for branch
1. merge the branch
1. return to terminal and if still in branch, navigate to main `git checkout main`
1. update version on local machine with `git pull origin main`
1. delete branch on github if desired with `git push origin --delete remoteBranchName`


## Jon Duckett HTML Book

## Chapter 5- Images (Pages 94-125)

The big idea: Use an `<img>` tag to add an inage to a page. There are **three** parts to an image element on your page.

1. The opening tag. There is no closing tag. 
1. The src. This is the source of the image, and tells the browser where the image is coming from. 
1. The alt. This provides a description of what is happening in the picture. 

`<img src="./img/flower.png" alt="A peony" />`

If you want to change the height and width directly on the image and not in the CSS, add `width="" height=""` before the tag ends. It is also possible to use `<figure>` to surround both an image and a `<figcaption>`

Images are **inline** elements. This means that they will display in the flow of other elements if placed inside other elements, and not necessarily on a new line.

### Rules for Creating Images (page 107)

1. Save in JPEG for natural scene or not a lot of variation
1. Save in PNG for images with sharp contrasts and transparency
1. Save in GIF for animations
1. Adjust the image size before adding to website
1. Use the right resolution (72 ppi)

### Final Facts

- *Scalable Vector Graphics* do not change quality as you increase their size. They are created with little dots, and are not bitmaps. 
- Each frame of a gif increases its size


## Chapter 11- Color (pages 246-263)

### Foreground

Three ways to specify color for text:

- RGB Values: `rgb(100,99,78)`
- Hex Codes: `#ee8e90`
- Color Names: `DarkCyan`

For all these options, the selector is the element whose text will take on these changes, and the property is `color`

### Background

Always set the background to some color. If that color is white, set `<body>` to white. 

### Contrast

Text must be readable, so contrast is a must. Low contrast is something to avoid- High contrast mixed with medium contrast is a good way to achieve balance. Increasing the spacing is helpful when text/background color is inverse.

### Opacity

To add opacity, one can use the **rgba** property instead of just rgb. The *a* represents opacity- and must be a value between 0.0 and 1.0.  
Or, simply use the property `opacity` and set the value. 

### hsla

By adding the letters `hsla` or `hsl` before a set of numbers following the background color property, one can control even more aspects of color.  

1. H = Hue = a degree between 0 and 360
1. S = Saturation = a percent between 0% and 100% (0 is gray, 100 is full color)
1. L = Lightness = a percent between 0% and 100% (0 is white, 100 is black)
1. A = Opacity = a number between 0 and 1.0 (0 is transparent, 100 is solid)


## Chapter 12- Text (pages 264-299)

### Terminology

- Serif = with details on the ends (Georgia, Times New Roman)
- Sans-Serif = straight ends (Calibri, Veranda)
- Monospace = every letter is same width
- Weight = thickness of text
- Style = angle of text (italic, oblique)
- Stretch = makes characters thin and close or wide and bolder

### Choosing a Typeface

Typefaces are subject to copyright!!! Be careful of what the licenses say. 

Designing from Mac --> PC, you need to check what the typefaces look like on other machines. 

### Specifying Typefaces

- Font-family = Specifies the typeface of text in an element
  - Typeface must be installed on user's computer to show
  - No more than 3 different ones on a page
- Font-size = Size can be specified in pixels (px), percentages (%), or ems. 

### Type Scales
 
Some designers set the main text of the body to 16 pixels, and scale everything around it based on that default. Here would be an example of heading sizes using 16px as the default:

- h1 = 32px
- h2 = 24px
- h3 = 18px
- body = 16px

Using pixels ensures that there is a lower likelihood the text will vary in size from browser to browswer. 

### Changes to Text Look

- **text-transform** = `uppercase` or `lowercase` or `capitalize` can all be applied to change the look of text
- **text-decoration** = `none` or `underline` or `overline` or `line-through` or `blink` (which makes text flicker)
- **line-height** = `___ em` and will change vertical gap between lines
- **letter-spacing & word-spacing** = `___ em` will change space between each letter, or between each word
- **text-align** 
  - `left` is easiest to read
  - `center` shifts it all to the middle
  - `justify` fills out the space of the box, and gives equal space to the area between each word in a given line. Good for paragraphs
- **vertical-align** = typically used with inline elements
- **text-indent** = `___ px` can take a negative value. 
- **text-shadow** = `1px 1px 0px #000000` gives a shadow to words
- **links**
  - a:link, a:visited, a:hover, a:active = all properties of links that can be targeted with color or text-decoration (underline)
- **interactive response**
  - :hover, :active, :focus = all pseudo-classes that can change interactive elements like buttons. Changes styling of elements when they are hovered over, being interacted with, or activated. 

### Attribute Selectors (page 292)

- `p[class]` matches a specific attribute
- `p[class ="card"]` matches attribute with value of "card"
- `p[class~="dog"]` targets value of "dog" in a list of space-separated words
- `p[attr^"c"]` applies to an element with an attribute with the first letter as c
- `p[attr*"do"] applies to an element with an attribute with the letters "do"
- p[attr$"g"] applies to an element with the last letter as g

[Home](https://peymade.github.io/reading-notes/)