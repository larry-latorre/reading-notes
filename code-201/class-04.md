# Readings: HTML Links, JS Functions, and Intro to CSS Layout

## Learn HTML

## Creating Hyperlinks

**To create a basic link, we wrap text or other content inside what element?**

`<a>` tag element and using the href attribute

`<p>`
  I'm creating a link to
  `<a href="https://www.mozilla.org/en-US/">`the Mozilla homepage`</a>`.
`</p>`

**The href attribute contains what information?**

The web address of the linked website.

**What are some ways we can ensure links on our pages are accessible to all readers?**

By adding the title attribute.

### CSS Layout

### CSS Layout: Normal Flow CSS Layout: Positioning

**What is meant by “normal flow”?**

The way elements on a webpage lay themselves out without any CSS.

**What are a few differences between block-level and inline elements?**

Block-level elements create a "block-level box" that typically spans the full width of their parent container. They stack vertically, one on top of the other, creating distinct sections or blocks in the layout.

Inline elements create an "inline box" that occupies only as much width as necessary for their content. They flow within the text, side by side, within the containing block.


**Static** positioning is the default for every html element.

**Name a few advantages to using absolute positioning on an element.**

Precise Placement: Absolute positioning allows you to specify the exact location of an element relative to its nearest positioned ancestor or the containing element.

Overlapping Content: Absolute positioning allows elements to overlap each other. This can be beneficial when you want to create effects like tooltips or pop-up dialogs that need to appear above other content on the page.

Design Flexibility: Absolute positioning provides flexibility in design, enabling you to create complex and creative layouts that may not be achievable using other positioning methods.

**What is a key difference between fixed positioning and absolute positioning?**
 The key difference is that fixed positioning is relative to the viewport, while absolute positioning is relative to a specified container or the viewport if no container is specified.

## Learn JS

### Functions – Reusable Blocks of Code

**Describe the difference between a function declaration and a function invocation.**

A function declaration defines a function, specifying its name, parameters, and code block. It essentially creates the function. On the other hand, a function invocation calls or executes a function by using its name and providing the necessary arguments. It uses the defined function to perform a specific task and can return a result or have other side effects in the program.

**What is the difference between a parameter and an argument?**

Parameters are part of the function's definition and specify what kind of data the function expects. Arguments are the actual values provided when the function is called, and they correspond to the parameters of the function.

### Miscellaneous

### 6 Reasons for Pair Programming

**Pick 2 benefits to pair programming and reflect on how these benefits could help you on your coding journey.**

Improved Code Quality
 When two individuals work together, they can catch each other's mistakes and help ensure that the code is of higher quality.

Knowledge Sharing and Learning
 Pair programming promotes knowledge sharing and learning. When two programmers collaborate, they bring their unique perspectives, experiences, and skill sets to the table. This allows for the exchange of ideas and solutions, which can help both individuals learn new techniques, coding patterns, and best practices.