# Readings: Problem Domain, Objects, and the DOM

## JavaScript Object Basics

**How would you describe an object to a non-technical friend you grew up with?**

In JavaScript, an object is like a container that holds different things, kind of like a box with labels. These labels are called "properties," and they help you organize and store information. Imagine you have a toy box with compartments for different toys, and each compartment has a name or label. You can put various toys (data) into these compartments, and you can also take them out when you need to play with or use them. Objects are handy for keeping related information together and easy to access.

**What are some advantages to creating object literals?**

Object literals are a convenient way to create and work with objects in JavaScript. Object literals in JavaScript offer simplicity, readability, and flexibility when working with objects.

**How do objects differ from arrays?**

Objects and arrays are both fundamental data structures, but they are used for different purposes. Objects are best suited for representing structured data with named attributes, while arrays are designed for storing and accessing ordered collections of data. The choice between objects and arrays depends on the specific requirements of your program and the nature of the data you are working with.

**Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.**

Bracket notation is used to access an object's property when the property name contains special characters, spaces, or when the property name is stored in a variable.

**Evaluate the code below. What does the term this refer to and what is the advantage to using this?**

const dog = {
  name: 'Spot',
  age: 2,
  color: 'white with black spots',
  humanAge: function (){
    console.log(`${this.name} is ${this.age*7} in human years`);
  }
}

The term this refers to the object to which the method belongs. In this case, this refers to the dog object. Using this inside the method allows you to access the object's properties within the method. This makes it easier to write code that can work with different instances of the dog object without having to hardcode specific property values.

### Introduction To The DOM

**What is the DOM?**

The Document Object Model (DOM) is a programming interface for web documents. It represents the structure of a web page, such as HTML or XML, as a tree-like structure where each node in the tree corresponds to part of the page's content. The DOM allows programmers to interact with and manipulate the content, structure, and style of a web page using a programming language like JavaScript.

**Briefly describe the relationship between the DOM and JavaScript.**

The DOM represents the document as a tree of objects, where each part of the web page (HTML elements, attributes) is represented as an object that can be accessed and manipulated using programming languages like JavaScript.
