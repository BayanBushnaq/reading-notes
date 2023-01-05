# What is global state with React?

### In the context of React, "global state" refers to data that is available to multiple components of a application, rather than being local state that is specific to a single component.

### There are several ways to manage global state in a React application. One common way is to use a state management library like Redux or MobX.

### consider a simple to-do list application with a list of tasks and a way to add new tasks. The list of tasks could be stored in global state, so that any component in the application can access the list and display it, or add new tasks to it.

### With Redux, you could store the list of tasks in a Redux store, and the components in your application could use the store to access the data. Here's an example of how you might set up the store and connect a component to it:


    import { createStore } from 'redux';

    // Define the reducer that handles updates to the store
        function todoReducer(state = [], action) {
        switch (action.type) {
            case 'ADD_TODO':
            return [...state, action.todo];
            default:
            return state;
        }
        }

        // Create the store with the reducer
        const store = createStore(todoReducer);

        // Connect a component to the store
        class TodoList extends React.Component {
        componentDidMount() {
            // Subscribe to the store to be notified of changes
            this.unsubscribe = store.subscribe(() => this.forceUpdate());
        }

        componentWillUnmount() {
            // Unsubscribe from the store to avoid memory leaks
            this.unsubscribe();
        }

        render() {
            // Get the current state from the store
            const state = store.getState();

            // Render the to-do list using the state
            return (
            <ul>
                {state.map((todo, index) => (
                <li key={index}>{todo.text}</li>
                ))}
            </ul>
            );
        }
        }
### With this setup, the TodoList component is connected to the Redux store, and will re-render whenever the store is updated. Other components in the application can also connect to the store and access the global state in the same way

# Context:

## What is the Context API in React?
### The Context API in React is a way to pass data through the component tree without having to manually pass props down the tree. It allows you to create a "context" that can be consumed by any component in the tree.

## Why is the Context API useful in a React application?
### The Context API is useful in a React application because it allows you to avoid prop drilling, which is the process of passing props down through multiple levels of components to reach the components that need the data. By using the Context API, you can make data available to any component in the tree without having to manually pass it down.

## How do I use the Context API in a React application?
### To use the Context API in a React application, you first need to create a context using the React.createContext function. Then, you can use the Provider component to provide the context to the component tree, and the Consumer component to consume the context.

# Redux vs Context API: When to use them ? 
## Redux and the Context API are both ways to manage global state in a React application, but they have different use cases and trade-offs.

### Here are some factors to consider when deciding whether to use Redux or the Context API:

 - Complexity: Redux is a more powerful and feature-rich state management solution, but it also requires more setup and has a steeper learning curve. The Context API, on the other hand, is simpler and easier to use, but it may not be sufficient for larger or more complex applications.

 - Scale: Redux is designed to scale to larger applications, and can handle complex state changes and updates. The Context API is more suitable for smaller applications or for cases where you need to pass data a few levels down the component tree.

 - Performance: In general, Redux has better performance than the Context API, because it uses a centralized store and a predictable update model. The Context API, on the other hand, can result in more re-renders and may have performance issues in large applications.

 - Ease of use: The Context API is generally easier to use than Redux, because it requires less setup and has a simpler API. However, Redux may be more suitable for applications with complex state management requirements.

### the choice between Redux and the Context API depends on the needs of your application. If you have a small or medium-sized application with simple state management needs, the Context API may be a good choice. If you have a larger or more complex application, or if you need advanced features like time-travel debugging or state persistence, Redux may be a better fit.