# Functional Programming

## Functional Programming Concepts

**What is functional programming?**

Functional programming (FP) is a programming paradigm that treats computation as the evaluation of mathematical functions and avoids changing state and mutable data. In functional programming, functions are first-class citizens, meaning they can be assigned to variables, passed as arguments to other functions, and returned as values from other functions.

**What is a pure function and how do we know if something is a pure function?**

A pure function is a function that, given the same input, will always produce the same output and has no side effects. This means that the function's behavior is entirely determined by its input parameters, and it does not rely on or modify external state. The absence of side effects ensures that calling a pure function doesn't cause any observable changes beyond the function's return value.

**What are the benefits of a pure function?**

Pure functions offer various advantages, including determinism, referential transparency, ease of testing, support for parallelization, memoization, improved maintainability, functional composition, and better support for concurrency and parallelism. They contribute to code that is more reliable, predictable, and modular, making it easier to reason about and maintain. However, achieving complete purity may not always be practical or necessary in all programming scenarios.

**What is immutability?**

Immutability is a programming concept where the state of an object, once set during creation, cannot be modified. Instead of altering the existing object, operations on immutable objects create new instances with the desired changes. This results in predictable, thread-safe, and easier-to-debug code. Immutability is often associated with functional programming and contributes to the development of reliable and maintainable software.

**What is Referential transparency?**

Referential transparency is a property of functions or expressions in programming where, given the same input, they always produce the same output and can be replaced with their computed values without altering the program's behavior. This property simplifies reasoning about code, allows for straightforward substitution, and is closely associated with the concept of pure functions in functional programming. Referentially transparent functions have no side effects, making code more predictable and easier to understand.

### Node JS Tutorial for Beginners #6 - Modules and require()

**What is a module?**

A module is a self-contained and reusable unit of code in programming that encapsulates related functions, variables, and data structures. It provides a way to organize and structure code, promoting modularity and reusability. Modules help manage complexity in larger software projects by breaking them into smaller, more manageable parts. They often include an interface that specifies how other parts of the program can interact with the module, hiding internal details and promoting a clear separation of concerns. Modules are a fundamental concept in modular programming and are used across various programming languages and paradigms.

**What does the word ‘require’ do?**

The term "require" is commonly used in programming to bring in external functionality or modules into a program. Its specific usage depends on the programming language or environment. In JavaScript (Node.js), it is used to import modules, in Ruby to load external libraries, and in Python, the equivalent is the `import` statement. The purpose is to include and make use of code defined in other files or libraries, promoting code organization, modularity, and reuse.

**How do we bring another module into the file the we are working in?**

To bring another module into the file you're working in, you typically use the `require` statement in Node.js (JavaScript/TypeScript) or the `import` statement in Python. In Node.js, you can also use the ECMAScript `import` syntax. The specific syntax may vary depending on the programming language and module system in use. This process allows you to access and use functionality defined in other files or modules, promoting code organization and modularity.

**What do we have to do to make a module available?**

To make a module available for use in your code, follow these steps:

1. **Create the Module:**
   - Write the code defining functions, variables, or classes in the module.

2. **Export the Module:**
   - Explicitly export elements (functions, variables, etc.) using appropriate export statements, making them accessible outside the module.

3. **Import the Module:**
   - In the file where you want to use the module, import it using the language-specific import or require statement.

This process allows you to organize and reuse code by making the functionality of a module accessible in different parts of your program. Examples in JavaScript (Node.js) and Python illustrate the creation, export, and import of modules.
