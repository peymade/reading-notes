# Reading 2

The reading for these notes can be found at [this link](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

## React Component Lifecycle Events

Lifecycle events are methods you can use on components. 

Based on the diagram, the very first thing that happens is the constructor, in the mounting phase. And the render happens before the componentDidMount. There is a render phase, a pre-commit phase, and a commit-phase. 

*Mounting* is when something is made and added to the DOM. 
*Updating* is when something has a change made to it and mush be rerendered. 
*Unmounting* is when something has already been added but must be removed from the DOM.

Order of events: constructor --> render --> React Updates --> componentDidMount & componentWillUnmount

### General Notes

- Do not use `this.setState()` in a constructor 
- `render()` is required in a class component
- `componentDidMount()` happens after a component has been mounted.Use for network request or DOM initialization. Could use it to connect with APIs. 
- `shouldComponentUpdate` is used to prevent components from rerendering every single time there is a state change, which is what will happen by default
- `componentDidUpdate()` is used for performing tasks after something is finished happening. 
- Unsafe lifecycle events should not be used.

## React States vs Props

1. What types of things can you pass in the props?  
Props are like arguments to a function. You can pass in text such as titles or descriptions, or things like values to use within the components as counters.
1. What is the big difference between props and state?  
Props are passed into a component and are updated outside the component, while state exists within, and is updated within. A change to a state triggers a re-rendering.
1. When do we re-render our application?  
When there is a change to a state. This is helpful for when the application should reflect a change each time a value updates.
1. What are some examples of things that we could store in state?
State can store user interaction information such as what value a person has selected out of checkboxes. 

If the information is static, use props. If information is dynamic, consider using state. 

## Things I want to know more about

I am curious as to when/why re-rendering would want to be prevented after a state change. 

[Home](https://peymade.github.io/reading-notes/)