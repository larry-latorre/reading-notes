# Putting it all together

 ## Thinking in React

**What is the single responsibility principle and how does it apply to components?**

The Single Responsibility Principle (SRP) is one of the SOLID principles of object-oriented design, and it states that a class (or, in the context of React, a component) should have only one reason to change. In other words, a component should have only one responsibility or job.

**What does it mean to build a ‘static’ version of your application?**

Building a "static" version of your application refers to creating a version of your application that doesn't have dynamic behavior or interactivity. In this context, "static" means that the content and layout are fixed and don't change based on user input or any external factors. It's essentially a snapshot of how your application looks with sample or predefined data.

**Once you have a static application, what do you need to add?**

Once you have a static version of your application, the next step is to add interactivity, dynamic data, and state management to make it a fully functional and dynamic application. 

**What are the three questions you can ask to determine if something is state?**

**Does it change over time?**

If the value or information can change during the lifecycle of the component or application, it is likely a candidate for state. State represents data that can be updated or modified as the application evolves.

**Is it passed from a parent component via props?**

If the data comes from a parent component and remains constant throughout the component's lifecycle, it might not need to be stored as state. However, if the value needs to be modified or updated within the component itself, it is likely state.

**Does it affect the rendering of the component?**

If the data influences the appearance or behavior of the component and changes in this data should trigger a re-render, it is a strong indicator that it should be managed as state. React components re-render when their state changes, updating the UI to reflect the new state.

**How can you identify where state needs to live?**

To identify where state needs to live in a React application:

Identify Components: Identify components that require dynamic data or user interaction.

Single Responsibility Principle: Ensure each component has a focused responsibility, separating display and state management.

Consider Hierarchy: Evaluate the component hierarchy to determine where shared state should live, lifting state to common ancestors when necessary.

Check for Shared State: Lift state to a common ancestor when multiple components need access to the same data.
Evaluate Data Change: Consider how data changes over time, and lift state when changes need to be shared across components.

Think About Data Source: Manage data from external sources, such as API calls or user input, as state.

Consider Lifecycle: If data needs to persist across multiple renders, manage it as state.

Reactivity Requirements: Use state for reactivity, enabling components to re-render when state changes.

### Higher-Order Functions

**What is a “higher-order function”?**

A higher-order function is a concept in programming where a function satisfies at least one of two conditions: it takes one or more functions as arguments or it returns a function as its result. Higher-order functions enable powerful abstractions, such as callbacks, function composition, and closures, contributing to modular, reusable, and expressive code. Examples include functions that accept callbacks for asynchronous operations or functions that return new functions for dynamic behavior. This concept is foundational in functional programming and widely used in languages like JavaScript.

### Explore the greaterThan function as defined in the reading.

 **In your own words, what is line 2 of this function doing?**

The arrow function checks if m is greater than the original value n

**Explain how either map or reduce operates, with regards to higher-order functions.**

map and reduce are higher-order functions in JavaScript that operate on arrays.

map Function

It iterates over each element of an array.
Applies a provided function to each element.
Creates a new array containing the results.
Does not mutate the original array.

reduce Function

It iterates over each element of an array.
Maintains an accumulator to accumulate results.
Applies a provided function to each element, updating the accumulator.
Produces a single value as the final result.
Does not mutate the original array.