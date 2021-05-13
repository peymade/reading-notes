# Reading 5

## Thinking in React [Link](https://reactjs.org/docs/thinking-in-react.html)

### General Notes

Do not use state more than you have to
Use the onChange event on inputs to notify when the user changes the input.


### How would you break a mock into a component heirarchy?

A mock design of a feature on a page should be broken down according to how many separate elements are within it. One could draw boxes around the different items that have different functionalities. 

### What is the single responsibility principle and how does it apply to components?

The *single responsibility principle* is the idea that, much like with functions, components should do one thing. For example, a 'renderImages' component should render the images, and not focus on doing too many other tasks.

### What does it mean to build a ‘static’ version of your application?

A static version is everything you want in your application, minus the interactivity. The interactivity can be layered on top once you have something you like. Do not use state in the static stage. 

### Once you have a static application, what do you need to add?

You need to add values that are dynamic (stored in state) so that things can actually change based on user interaction. 

### What are the three questions you can ask to determine if something is state?

(These questions come directly from the React doc linked at the top of this page)

If the answer it yes to any of these questions, it is likely not state.
- Is it passed in from a parent via props?
- Does it remain unchanged over time?
- Can you computer it based on any other state or props in your component?

### How can you identify where state needs to live?

Follow these steps:

- Identiy which components render things based on this state
- Find a parent to all these components that want to render the same thing
- This parent component should be where state is placed


[Home](https://peymade.github.io/reading-notes/)