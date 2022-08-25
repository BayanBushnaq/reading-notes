# React Docs - Thinking in React 

## What is the single responsibility principle and how does it apply to components?
###  a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents

## What does it mean to build a ‘static’ version of your application?
### a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props.

## Once you have a static application, what do you need to add?
### static version requires a lot of typing and no thinking, and adding interactivity requires a lot of thinking and not a lot of typing.

## What are the three questions you can ask to determine if something is state?
- Is it passed in from a parent via props? If so, it probably isn’t state.
- Does it remain unchanged over time? If so, it probably isn’t state.
- Can you compute it based on any other state or props in your component? If so, it isn’t state.
- 
## How can you identify where state needs to live?
### we have identified what the minimal set of app state is. Next, we need to identify which component mutates, or owns, this state.

# Higher-Order Functions
## What is a “higher-order function”?
### a function that takes a function as an argument, or returns a function 

## Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
### I think it's mean if this component is a parent for another one!

