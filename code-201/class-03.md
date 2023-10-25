# Learn HTML

## Ordered and Unordered lists.

**When should you use an unordered list in your HTML document?**

If there is no need or meaning to the order.

**How do you change the bullet style of unordered list items?**

You can change the bullet style using the list-style-type property in your CSS. 

**When should you use an ordered list vs an unorder list in your HTML document?**

 The choice between using an ordered list or an unordered list depends on the nature of the content you want to display.

**Describe two ways you can change the numbers on list items provided by an ordered list?**

You can change the style of the numbers in an ordered list using the CSS list-style-type property.
You can also customize the appearance of the number marker by using the ::before pseudo-element. 

### Learn CSS

The Box Model.

**Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: “The Box Model”?**

In the enchanting tale of "The Box Model," Margin and Padding are two essential characters who play pivotal roles in shaping the narrative. Margin is the friendly and accommodating character who creates space between the elements, ensuring that they have a comfortable distance from one another. Padding, on the other hand, is the protective and supportive figure, providing a cushioning layer inside each element to shield its content from the outside world. Together, Margin and Padding work harmoniously to define the boundaries and spacing of every element in the story, ensuring that the layout remains balanced and visually appealing. Their dynamic interplay is a cornerstone of the box model, ultimately contributing to the story's design and presentation.

Source Chat GPT.

**List and describe the four parts of an HTML elements box as referred to by the box model.**

Content: The content is the innermost part of an HTML element's box.

Padding: Padding is the space between the content and the element's border. It is used to create space around the content.

Border: The border is a line that surrounds the padding and content of an HTML element. It helps define the boundaries of the element.

Margin: Margin is the space outside an HTML element's border. It separates the element from other elements on the page.

## Learn JS

### Arrays. Operators and Expressions. Conditionals. Loops

**What data types can you store inside of an Array?**

Numbers: This includes integers and floating-point numbers.

Strings: You can store text and characters in array elements.

Booleans: You can store true and false values in an array.

Objects: JavaScript objects, including custom objects and built-in objects like Date and RegExp, can be elements in an array.

Functions: You can store JavaScript functions in an array.

Arrays: You can nest arrays inside other arrays, creating multi-dimensional arrays.

Undefined: If an array element has not been assigned a value, it will hold the special value undefined.

Null: You can also store the value null in an array.

Symbols: If your JavaScript environment supports ES6 Symbols, you can store them in an array.

NaN: Not a number

**Is the people array a valid JavaScript array? If so, how can I access the values stored? If not, why?**

 const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];

 Yes it is a valid array. You can access the values stored by using the index position of the array or index position of the value within the array.

**List five shorthand operators for assignment in javascript and describe what they do.**

+= Addition Assignment
Description: This operator adds the value on the right hand side to the variable on the left hand side  and assigns the result back to the variable. 

-= Subtraction Assignment

Description: This operator subtracts the value on the right hand side from the variable on the left-hand side and assigns the result back to the variable.

*= Multiplication Assignment

Description: This operator multiplies the variable on the left hand side by the value on the right hand side and assigns the result back to the variable.

/=: Division Assignment

Description: This operator divides the variable on the left hand side  by the value on the right hand side and assigns the result back to the variable.

%=: Modulus Assignment

Description: This operator computes the remainder of the division of the variable on the left hand side  by the value on the right hand side and assigns the remainder as the new value of the variable.

**Read the code below and evaluate the last expression and explain what the result would be and why.**

 let a = 10;
 let b = 'dog';
 let c = false;

 // evaluate this
 (a + c) + b;

a is a number, b is a string and c is a boolean.

a = 10 c = 0 because false is equal to zero. So 10 + 0 = 10. Now you have 10 + 'dog' which can be concatenated to 10dog.
**Describe a real world example of when a conditional statement should be used in a JavaScript program.**

You could use a conditional statement for stop lights. If there are a certain amount of cars waiting to go change signal to green.

**Give an example of when a Loop is useful in JavaScript.**

Loops are useful in JavaScript for repetitive tasks, such as iterating through arrays, processing data, and performing actions multiple times.