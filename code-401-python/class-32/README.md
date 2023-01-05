# Building Your Own Hooks : 
## -  Hooks are a feature in React that allow you to reuse stateful logic across components.
 *  You can extract this logic into a custom hook, which is a function whose name starts with "use" and that may call other hooks.

 *  The main advantage of custom hooks is that they allow you to share logic across multiple components and keep your codebase DRY.

 *  In the example provided, the useFriendStatus hook is used to subscribe to a friend's status and return whether they are online or not. The hook takes the friend's ID as an argument and uses the useState and useEffect hooks to update the status and subscribe/unsubscribe to the status changes. 

 * The hook is then used in the FriendStatus and FriendListItem components to display the friend's status.

 * To use a custom hook, you can call it like a normal function in your component and use the returned value. 

 * Custom hooks are a useful way to abstract away complex logic and make your components more readable and reusable.

# Lifting State Up : 
 * In React, the concept of "lifting state up" refers to the idea of moving shared state to the component higher up in the tree that needs it, rather than having it managed independently by each component that uses it.

 *  This is useful when you have several components that need to reflect the same changing data. An example given in the documentation is a temperature calculator with inputs for both Celsius and Fahrenheit, and a component that calculates whether the water would boil at a given temperature.

 * To keep the inputs in sync, the shared state (the temperature) should be moved up to their closest common ancestor (in this case, the Calculator component). 

 * The Calculator component can then pass the temperature down as a prop to the input components and the BoilingVerdict component, and handle any changes to the temperature itself. 

 * This way, the input components don't have to worry about storing or converting the temperature, and the BoilingVerdict component can simply accept the temperature as a prop.

# Thinking in React:

## The process of building a searchable product data table using React involves several steps:

 - 1- Breaking the UI into a component hierarchy: Identify the different components needed in the app by drawing boxes around each one in the mock and giving them names. Use the single responsibility principle to decide if a component should be decomposed into smaller subcomponents.

 * 2- Building a static version in React: Create a version of the app that takes the data model and renders the UI, but has no interactivity. Use props to pass data from parent to child components.

 * 3- Identify the minimal (but complete) representation of UI state: Determine what state is necessary for the app to render the UI, and where it should be stored. This may involve adding state to some or all of the components in the hierarchy.

 * 4- Identify where your state should live: Decide which component should own the state, and where the state should be initialized.

 * 5- Add inverse data flow: Implement the logic for changing the state, and ensure that the data flows correctly from the stateful component to the child components that render the UI.

* 6- Add server communication: Set up the app to retrieve data from the JSON API and use it to populate the UI.

 * 7- Add routing: If the app has multiple pages, add routing to navigate between them.

# MEMOIZATION IN REACT JS  :

### Memoization is a technique used to improve the performance of a program by storing the results of expensive function calls, so that they can be reused when the same inputs are given in the future.

### In React, memoization can be implemented using either the PureComponent class or the memo hook.

### The PureComponent class is similar to the regular Component class, but it implements the shouldComponentUpdate() method with shallow prop and state comparison.

### This allows it to skip re-rendering if the props and state remain unchanged. 
### The memo hook allows memoization to be applied to functional components, by wrapping the component in a higher-order component (HOC) that stores and reuses the last rendered result.
### The default behavior of memo is to shallowly compare the props object, but a custom comparison function can be passed as a second argument to control this behavior.
### Memoization can be useful in cases where a component is re-rendering the same result with the same props and state, which can cause performance issues.
### By applying memoization, the component can skip the re-render and improve performance.
