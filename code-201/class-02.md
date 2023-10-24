# HTML Text Fundamentals. HTML Advanced Text Formatting.

**Why is it important to use semantic elements in our HTML?**

Semantic elements not only improves accessibility for users with disabilities but also benefits search engines in indexing and ranking web pages accurately. Also, semantic HTML makes code more readable and maintainable for developers.

**How many levels of headings are there in HTML?**

In HTML, there are six levels of headings.

**What are some uses for the `<sup>` and `<sub>` elements?**

The `<sup>` and `<sub>` elements in HTML are used to control the vertical alignment and formatting of text or other inline elements.

**When using the `<abbr>` element, what attribute must be added to provide the full expansion of the term?**

When using the `<abbr>` element in HTML, you should include the title attribute to provide the full expansion or explanation of the abbreviated term.

## Learn CSS

**How CSS Is Structured.**

The basic structure of CSS:

* Selector

* Declaration Block

* Property

* Value

**What are ways we can apply CSS to our HTML?**

Inline CSS:

`<p style="color: red; font-size: 16px;">`This is a red, 16px text.`</p>`

Internal CSS:

`<head>`
  `<style>`
    p {
      color: blue;
      font-size: 18px;
    }
  `</style>`
`</head>`

External CSS:

In your HTML file

`<head>`
  `<link rel="stylesheet" type="text/css" href="styles.css">`
`</head>`

In your styles.css file:

p {
  color: green;
  font-size: 20px;
}

**Why should we avoid using inline styles?**

Inline styles can make your code less maintainable and harder to manage.  Inline styles can also hinder the reusability of styles across your website

**Review the block of code below and answer the following questions:**

   h2 {
     color: black;
     padding: 5px;
   }

**What is representing the selector?**

h2

**Which components are the CSS declarations?**

color: black;
padding: 5px;

**Which components are considered properties?**

color and padding