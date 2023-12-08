# In memory storage

## Understanding the JavaScript Call Stack

**What is a ‘call’?**

In the context of the JavaScript Call Stack, a "call" refers to the invocation or execution of a function. When you invoke a function in JavaScript, it creates a new frame on the call stack to keep track of the function's execution context. This frame contains information such as the local variables, parameters, and the location in the code where the function was called from.

**How many ‘calls’ can happen at once?**

In JavaScript, the number of concurrent function calls is influenced by the language's single-threaded, event-driven model. JavaScript achieves concurrency through mechanisms such as asynchronous programming and Web Workers. Asynchronous operations, managed by the event loop, enable non-blocking execution, allowing multiple tasks to progress simultaneously. Web Workers provide true parallelism by running scripts in the background. However, practical limits on concurrency depend on factors like the runtime environment, system resources, and task complexity. While JavaScript is single-threaded, it can effectively handle multiple operations through asynchronous programming, enabling responsiveness in applications.

**What does LIFO mean?**

LIFO stands for "Last In, First Out." It is a principle applied in various contexts, including data structures and accounting. In the context of data structures, LIFO is associated with stacks, where the last item added is the first one to be removed. This principle is also applied in memory management, such as the call stack in programming languages. Additionally, LIFO is a method used in financial accounting for inventory valuation, where the most recently acquired items are considered the first to be sold or used. The opposite of LIFO is FIFO, which stands for "First In, First Out."

**Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.**

|---------------------|
|        main()       |   <--- Top of the stack
|---------------------|
|   firstFunction()   |
|---------------------|
|  secondFunction()   |
|---------------------|   <--- Current state

**What causes a Stack Overflow?**

A stack overflow occurs when the call stack of a program exceeds its allocated size due to factors such as infinite recursion, deep recursion, large local variables, or infinite loops. This results in a runtime error and can be challenging to debug. Properly designing functions with appropriate termination conditions is essential to prevent stack overflow issues. Understanding the structure and limits of the call stack is crucial for identifying and addressing these issues in programming.

### JavaScript error messages

**What is a ‘reference error’?**

A "ReferenceError" in programming, such as in JavaScript, occurs when attempting to reference a variable or function that has not been declared or is outside the current scope. This error is commonly encountered when using undeclared variables, misspelling variable or function names, or accessing properties on undefined objects. Identifying and correcting these issues is crucial for debugging and ensuring the proper execution of the code.

**What is a ‘syntax error’?**

A "syntax error" is a programming error detected during the parsing phase, before the execution of the code. It occurs when the code violates the syntactical rules of the programming language. Examples include missing or mismatched parentheses, brackets, or braces, missing semicolons, misspelled keywords, and incorrect variable or function declarations. Syntax errors must be corrected to ensure the proper structure and adherence to the language's syntax rules. They are typically identified early in the development process during code compilation or interpretation.

**What is a ‘range error’?**

A "RangeError" in programming occurs when a value is not within the acceptable range as defined by the programming language or a specific function. This error is thrown at runtime when an operation leads to a value outside the allowed range. Examples include attempting to create an array with a negative length, performing mathematical operations with extremely large or small values, or using excessively large lengths for strings. RangeErrors indicate that the program is trying to perform an operation that is not valid due to the provided values being outside the acceptable range.

**What is a ‘type error’?**

A 'type error' in programming occurs when an operation is performed on a data type that is not supported or compatible with that operation. It happens when attempting to use a variable or value in a way that is not allowed for its data type. For example, trying to add a string and an integer without proper conversion may result in a type error. Programming languages often have mechanisms to catch and handle these errors to prevent unexpected behavior or crashes in a program.

**What is a breakpoint?**

A breakpoint is a debugging tool that allows developers to pause the execution of a program at a specific point in the code. This feature enables them to inspect variables, step through code, isolate issues, and make on-the-fly changes, making it easier to identify and resolve bugs during the debugging process. Breakpoints are set using integrated development environments (IDEs) or debugging tools provided by programming languages.

**What does the word ‘debugger’ do in your code?**

A debugger is a software tool used in programming to identify and fix bugs in code. It provides features such as setting breakpoints to pause execution, stepping through code, examining variables, watching expressions, using conditional breakpoints, inspecting the call stack, and examining memory. Debuggers assist developers in efficiently locating and resolving issues during the development process, improving the overall quality of the code. They are often integrated into development environments or available as standalone tools for different programming languages.
