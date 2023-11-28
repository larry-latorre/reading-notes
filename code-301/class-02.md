# Readings: State and Props

## React lifecycle

**Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?**

The render method is called before the componentDidMount method.

**What is the very first thing to happen in the lifecycle of React?**

In the lifecycle of a React component, the very first thing to happen is the Initialization or Construction phase. This is when the component is created and initialized. The constructor of the component is called during this phase. If you're using the constructor method in your component, it's the first method that gets executed.

**Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates.**

The constructor, render, componentDidMount, for the initial mount, and if the component updates, it goes through the React update process, followed by possible re-rendering and updates, and finally, if the component is unmounted, componentWillUnmount is called.

**What does componentDidMount do?**
The componentDidMount lifecycle method in a React class component is invoked immediately after a component is inserted into the DOM (Document Object Model). It is a good place to perform tasks that require interaction with the DOM or external data fetching, as it ensures that the component has been rendered to the DOM.

### React State Vs Props

**What types of things can you pass in the props?**

The componentDidMount lifecycle method in a React class component is invoked immediately after a component is inserted into the DOM (Document Object Model). It is a good place to perform tasks that require interaction with the DOM or external data fetching, as it ensures that the component has been rendered to the DOM.

**What is the big difference between props and state?**

Props:

- Passed from parent to child components.
- Immutable (read-only) data.
- Owned and set by the parent component.
- Used for one-way communication from parent to child.
- Initialized by the parent component when the child is created.
- Changes in props trigger re-rendering of the child component.

State:

- Managed internally within a component.
- Mutable (can be changed) data.
- Owned and managed by the component itself.
- Used for handling dynamic data, user interactions, and changes within a component.
- Initialized in the constructor of a class component or using useState in a functional component.
- Changes in state trigger re-rendering of the component.

**When do we re-render our application?**

In React, a re-render of a component occurs when the component's state or props change. React automatically handles the process of determining when to re-render components based on changes in their state or props.

**What are some examples of things that we could store in state?**

In React, the component's state is used to manage and store dynamic, mutable data within a component. Here are some common examples of things you might store in the state:

**User Input:**

Capture and manage user input, such as form values.

**Toggle States:**

Manage boolean values for toggling the visibility or activation of elements or features.

**API Data:**

Store data fetched from APIs, enabling dynamic updates based on external data.

**Error Handling:**

Manage error messages to handle and display errors gracefully.
