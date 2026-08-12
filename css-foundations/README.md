# CSS foundations

### Lesson overview

This section contains a general overview of topics that you will learn in this lesson.

1. Adding styles to HTML with CSS.
2. How to use the class and id attributes.
3. How different CSS selectors work.

There are three ways to add CSS to HTML:

- External CSS
- Internal CSS
- Inline CSS

### External CSS

External CSS is the most common method you will come across, and it involves creating a separate file for CSS and linking it inside the HTML.

`<link rel="stylesheet" href="styles.css">`

### Basic syntax

At the most basic level, CSS is made up of various rules. Each rule is made up of a selector (more on this in a bit) and a semicolon-separated list of declarations, with each of those declarations being made up of a property–value pair.

### Selectors

Selectors refer to the HTML elements to which CSS rules apply; they’re what is actually being “selected” for each rule. The following subsections don’t cover every selector available, but they’re by far the most common and the ones you should get comfortable using first.

As you go through each example, play around with them to see the results by adding both the HTML and CSS to their respective files.

### Universal selector

The universal selector will select elements of every type (as in the whole document), hence the name “universal”, and the syntax for it is a simple asterisk. In the example below, every element would have the `color: purple;` style applied to it.

### Type selectors

A type selector (or element selector) will select all elements of the given element type, and the syntax is just the name of the element:
`div {color:white;} `

### Class selectors

Class selectors will select all elements with the given class, which is just an attribute you place on an HTML element. Here’s how you add a class to an HTML tag and select it in CSS:
`.alert-text {color: red;}`

Another thing you can do with the class attribute is to add multiple classes to a single element as a space-separated list, such as `class="alert-text severe-alert"`. Since whitespace is used to separate class names like this, you should never use spaces for multi-worded names and should use a hyphen instead.

### ID selectors

ID selectors are similar to class selectors. They select an element with the given ID, which is another attribute you place on an HTML element. The major difference between classes and IDs is that an element can only have one ID. It cannot be repeated on a single page and should not contain any whitespace:
`#title {
  background-color: red;
}`

For IDs, instead of a period, we use a hashtag immediately followed by the case-sensitive value of the ID attribute. A common pitfall is people overusing the ID attribute when they don’t necessarily need to, and when classes will suffice. While there are cases where using an ID makes sense or is needed, such as taking advantage of specificity or having links redirect to a section on the current page, you should use IDs sparingly (if at all).
