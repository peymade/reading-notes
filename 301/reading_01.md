# Reading 1

## Component Based Architecture

These notes come from an article on tutorialspoint. [Link](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)

### What is a component?

A component is a section of code that can be reused. It is a sub-section of a larger section of code, and has an individual purpose.

### Views of a Component

*Object-oriented*: Each component is "a set of one or more cooperating classes." 

*Conventional*: Each component is a functional element or module. There may be functions, but things are not grouped together using objects. 

*Process-related*: Components are not all created by the developer, but may exist in a library, where they can be accessed and used.

### What are the charactistics of a component?

1. Resusability: it is typical for components to be designed for use in multiple situations in multiple apps.
1. Replaceable: components are not too specific where they can't be replaced by other similar chunks of code
1. Not context specific: designed for a variety of situations 
1. Extensible: components can be extended to build upon behavior that has already been built
1. Encapsulated: internal data, processes, or variables, are not exposed in components
1. Independent: generally have little dependancy on other pieces of the code

### Using Component Level Design

- Create a consistent naming convention for components
- Organize functionality into different sections that can be components independent of one another
- Map how each component relates to others, and what the dependencies are

### What are the advantages of using component based architecture?

By using component architecture, it makes deployment easier, because with functionality separated into components, it is easier to replace and update sections of the code. This simplifies maintenance, too. Third-party components also decrease development and maintenance costs, and make the development process easier by letting code be reused. Systems created with this architecture have increased reliability, since the components must be reliable and functional on their own. 

## Props in React

These notes come from an article by Cem Eygi. [Link](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0#:~:text=%E2%80%9CProps%E2%80%9D%20is%20a%20special%20keyword,way%20from%20parent%20to%20child)


### How are props used in React?

Props, short for properties, is how data is passed between components. Since React is a component-based library, it is important that those components have ways to communicate with each other. 

The data flow is downwards and unidirectional, and the data should not be changed by child components. 

To use Props, create the attribute and the data associated with it, pass it to the child using Props, and render it. Props are passed to components like arguments into a function. 

## Things I want to know more about

How many programming languages are object-oriented? Is this the most common structure for a programming language?

[Home](https://peymade.github.io/reading-notes/)