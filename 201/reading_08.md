# Reading 8

## Jon Duckett's HTML Book Chapter 15: layout

### Summary of previous notes on this chapter

- There are block level and inline elements. You can change one type to act like another. 
- Normally, block level elements stack one on top of another. You can change the positioning:
  - `position: relative` Moves block from normal flow, other elements unaffected
  - `position: absolute` Moves from normal flow, other elements fill in
  - `position: fixed` Sits in relation to browser window, does not move when scrolling
- Use `float` to move elements. If you use float, the space that it was moved from will be filled in with other elements. 
- Fixed width layout does not respond to changes in browser size- measurments could be in pixels
- Liquid layout responds to changes in browser size- measurments could be in percentages 


### Grids

A grid widely used by designers is the 960 pixel grid. Using a grid helps set proportions, makes it easier to create new pages with its template, and improves continuity. 
In a 960 pixel grid, there are 12 columns of 60 pixels, with 10 pixels of margin. Creating boxes/rectangles and splitting up the screen according to these columns is good. 

### CSS Frameworks

CSS Frameworks can be used to save time and code, and can provide built-in frameworks one can use to design a page more easily. In using the 960 pixel framework, one edits the HTML to assign elements to classes that take up different numbers of columns. For example, you may give a div element that contains the information on the page a "container_12" class attribute, which would signal to the CSS that you are using a 12 column grid, and the columns are to be created based on that container element. Then you could give a child element of that div element the class attribute: "grid_5," and you could create a block that is 5 columns wide. 


[Home](https://peymade.github.io/reading-notes/)