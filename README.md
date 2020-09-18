# Roadmap

---

## Contents

1. [Introduction](#Introduction)
2. [HTML](#HTML)
3. [CSS](#CSS)
4. [JavaScript](#JavaScript)
5. [Git](#Git)
6. [CLI](#CLI)
7. [Frameworks, Libraries, Preprocessors, Compilers](#Frameworks)
8. [CS Fundamentals](#CSFundamentals)

---

## [Introduction](#Introduction)

This is my personal roadmap for learning web development — specifically the front-end. This is heavily based on [Web Developer Roadmap](https://github.com/kamranahmedse/developer-roadmap), but may deviate from the original as I add more specificity.

## [HTML](#HTML)

### Semantic Structure

### Accessibility

### Study Concepts

What does a `doctype` do?

```html
All HTML documents must start with a <!DOCTYPE > declaration. The declaration is not an HTML tag. It
is an "information" to the browser about what document type to expect.
```

- How do you serve a page with content in multiple languages?

```html
Language can be set/prioritized through http request headers, with more prioritized languages given
greater “weight”. This can also be set with the “lang” attributes: 1 Define a primary language with
the lang attribute, and then call out the secondary language(s) with lang attributes on elements in
the document 2 Define lang in the specific sections of the document as needed
```

- What kind of things must you be wary of when designing or developing for multilingual sites?

```javascript
* Always use the lang and the dir attributes in all your HTML
* Avoid talking about "right side" and "left side"
* Don't ever concatenate translated strings:
"The date today is " + date
Rather add parameter support to your messages and do something like:
messages.date = "The date today is %date"... and then:msg( 'messages.date' );
```

- What are `data-` attributes good for?

```html
Data that should be associated with a particular element but need not have any defined meaning. Ex:
<!-- Extra Info about “#electric-cars” -->
<article id="electric-cars" data-columns="3" data-index-number="12314" data-parent="cars"></article>
```

```javascript
// JavaScript Access
const article = document.querySelector("#electric-cars");
// Can get and/or set
article.dataset.columns; // "3"
article.dataset.indexNumber; // "12314"
article.dataset.parent; // "cars"
```

```css
/* CSS Access */
article::before {
  content: attr(data-parent);
}

article[data-columns="3"] {
  width: 400px;
}
article[data-columns="4"] {
  width: 600px;
}
```

- Consider HTML5 as an open web platform. What are the building blocks of HTML5?

```html
• Semantics: allowing you to describe more precisely what your content is. • Connectivity: allowing
you to communicate with the server in new and innovative ways. • Offline and storage: allowing
webpages to store data on the client-side locally and operate offline more efficiently. •
Multimedia: making video and audio first-class citizens in the Open Web. • 2D/3D graphics and
effects: allowing a much more diverse range of presentation options. • Performance and integration:
providing greater speed optimization and better usage of computer hardware. • Device access:
allowing for the usage of various input and output devices. • Styling: letting authors write more
sophisticated themes.
```

- Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.

```html
localStorage, sessionStorage, and cookies are all client storage solutions. ￼* localStorage: *
sessionStorage: * cookies:
```

- Describe the difference between `<script>`, `<script async>` and `<script defer>`.

```html
<script></script>
```

- Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?
- What is progressive rendering?
- Why you would use a `srcset` attribute in an image tag? Explain the process the browser uses when evaluating the content of this attribute.
- Have you used different HTML templating languages before?

---

## [CSS](#CSS)

### - Flexbox

### - Grid

### - Hierarchy & Inheritance

---

## [JavaScript](#JavaScript)

### Study Concepts

- Explain event delegation.
- Explain how `this` works in JavaScript.
  - Can you give an example of one of the ways that working with `this` has changed in ES6?
- Explain how prototypal inheritance works.
- What's the difference between a variable that is: `null`, `undefined` or undeclared?
  - How would you go about checking for any of these states?
- What is a closure, and how/why would you use one?
- What language constructions do you use for iterating over object properties and array items?
- Can you describe the main difference between the `Array.forEach()` loop and `Array.map()` methods and why you would pick one versus the other?
- What's a typical use case for anonymous functions?
- What's the difference between host objects and native objects?
- Explain the difference between: `function Person(){}`, `var person = Person()`, and `var person = new Person()`?
- Explain the differences on the usage of `foo` between `function foo() {}` and `var foo = function() {}`
- Can you explain what `Function.call` and `Function.apply` do? What's the notable difference between the two?
- Explain `Function.prototype.bind`.
- What's the difference between feature detection, feature inference, and using the UA string?
- Explain "hoisting".
- Describe event bubbling.
- Describe event capturing.
- What's the difference between an "attribute" and a "property"?
- What are the pros and cons of extending built-in JavaScript objects?
- What is the difference between `==` and `===`?
- Explain the same-origin policy with regards to JavaScript.
- Why is it called a Ternary operator, what does the word "Ternary" indicate?
- What is strict mode? What are some of the advantages/disadvantages of using it?
- What are some of the advantages/disadvantages of writing JavaScript code in a language that compiles to JavaScript?
- What tools and techniques do you use debugging JavaScript code?
- Explain the difference between mutable and immutable objects.
  - What is an example of an immutable object in JavaScript?
  - What are the pros and cons of immutability?
  - How can you achieve immutability in your own code?
- Explain the difference between synchronous and asynchronous functions.
- What is event loop?
  - What is the difference between call stack and task queue?
- What are the differences between variables created using `let`, `var` or `const`?
- What are the differences between ES6 class and ES5 function constructors?
- Can you offer a use case for the new arrow `=>` function syntax? How does this new syntax differ from other functions?
- What advantage is there for using the arrow syntax for a method in a constructor?
- What is the definition of a higher-order function?
- Can you give an example for destructuring an object or an array?
- Can you give an example of generating a string with ES6 Template Literals?
- Can you give an example of a curry function and why this syntax offers an advantage?
- What are the benefits of using `spread syntax` and how is it different from `rest syntax`?
- How can you share code between files?
- Why you might want to create static class members?
- What is the difference between `while` and `do-while` loops in JavaScript?

---

## [Git](#Git)

---

## [CLI](#CLI)

---

## [Frameworks, Libraries, Preprocessors, Compilers](#Frameworks)

### JS Frameworks

#### - jQuery

#### - React

#### - Vue

#### - Angular

#### - Node

### CSS Libraries

#### - Materialize

#### - Skeleton

#### - Bootstrap

### CSS Preprocessors

#### - LESS

#### - SASS/SCSS

---

## [CS Fundamentals](#CSFundamentals)

### Algorithms & Data Structures

---

_To Do:_

- Test Build process for gh-pages deployment
- Create main page with checked/unchecked boxes to track progress
- Create documentation
