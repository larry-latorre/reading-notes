# React and Forms

## How to use Forms in React

**What is a ‘Controlled Component’?**

In React, a "controlled component" refers to a form element whose value is controlled by React state. In other words, the component doesn't maintain its own internal state for the value; instead, it receives the current value from the React state and notifies changes back to the parent component through a callback function.

**Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.**

The decision depends on the specific needs of your application and the desired user experience. It's not uncommon to find a balance—providing real-time feedback for simple forms and waiting until submission for more complex ones. Always consider the trade-offs and choose an approach that aligns with the goals of your application and the expectations of your users.

**How do we target what the user is entering if we have an event handler on an input field?**

In React, when you have an event handler on an input field, you can access the value that the user is entering through the event object passed to the event handler function. The value entered by the user is typically available through event.target.value.

### The Conditional (Ternary) Operator Explained

**Why would we use a ternary operator?**

A ternary operator is a concise way to write a conditional expression in many programming languages, including JavaScript. It's often used for making decisions and assigning values based on a condition.

**Rewrite the following statement using a ternary statement:**

if(x===y){
  console.log(true);
} else {
  console.log(false);
}

console.log(x === y ? true : false);
