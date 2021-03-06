![Roadmap Logo](src/assets/img/Roadmap_Logo.png)

![GitHub last commit](https://img.shields.io/github/last-commit/timmybytes/roadmap) ![GitHub](https://img.shields.io/github/license/timmybytes/roadmap) ![GitHub top language](https://img.shields.io/github/languages/top/timmybytes/roadmap) ![Snyk Vulnerabilities for GitHub Repo](https://img.shields.io/snyk/vulnerabilities/github/timmybytes/roadmap) ![Twitter Follow](https://img.shields.io/twitter/follow/timmybytes?style=social)

## About

This is my personal roadmap for learning web development — specifically the **front-end**. This guide started out as notes I was taking on the [Web Developer Roadmap](https://github.com/kamranahmedse/developer-roadmap) and [Front-end Interview Questions](https://github.com/h5bp/Front-end-Developer-Interview-Questions) while self-learning web development. I'm trying to combine (and expand) them into as comprehensive and inclusive a guide as possible for newbies and anyone interested in learning more about development in-depth. This is definitely a **work-in-progress**, and more will be added to these concepts as time allows.

If you're interested in adding anything, feel free to submit a Pull Request.

> 09/20/20: I'm in the process of building a live webpage for this, to make things more easy to navigate. It's being built with the [Sierra SCSS Library](https://sierra-library.github.io/#components) from @JoanClaret.

## [Contents](#Contents)

1. [Introduction](#Introduction)
   - [Web Development: Front, Back, and Full-Stack](#WebDev)
   - [Web Development Basics](#Basics)
2. [HTML](#HTML)
   - [Semantic Structure & Accessibility](#Semantic)
3. [CSS](#CSS)
4. [JavaScript](#JavaScript)
5. [Git](#Git)
6. [CLI](#CLI)
7. [Frameworks](#Frameworks)
8. [Stacks](#Stacks)
9. [Fundamentals](#Fundamentals)

## [Introduction](#Introduction)

### [Web Development: Front, Back, and Full-Stack](#WebDev)

There are a lot of terms that get thrown around in relation to people who write code that involves the Internet — Developer, Engineer, Architect, Specialist, etc. — and like a lot of the tech industry, the roles of these positions varies across organizations. Typically though, you can think of there being three _main_ (not exhaustive) areas:

- **Front-end**: This typically involves UI/UX (User Interfaces/User Experiences) that heavily involves the visual and interactive parts of the web. This might be building (and sometimes designing) websites, creating web apps, and any number of tasks related to the "front" facing parts of the web. **This guide focuses on the Front-end**.

- **Back-end**: ...

- **Full-stack**: ...

### [Web Development Basics](#Basics)

- ...

[Back to Contents](#Contents)

## [HTML](#HTML)

...

### [Semantic Structure & Accessibility](#Semantic)

- ...

### Study Concepts

#### What does a `doctype` do?

All HTML documents must start with a <!DOCTYPE > declaration. The declaration is not an HTML tag. It
is an "information" to the browser about what document type to expect.

#### How do you serve a page with content in multiple languages?

Language can be set/prioritized through http request headers, with more prioritized languages given
greater “weight”. This can also be set with the “lang” attributes: 1 Define a primary language with
the lang attribute, and then call out the secondary language(s) with lang attributes on elements in
the document 2 Define lang in the specific sections of the document as needed

#### What kind of things must you be wary of when designing or developing for multilingual sites?

- Always use the `lang` and the `dir` attributes in all your HTML
- Avoid talking about "right side" and "left side"
- Don't ever concatenate translated strings. Ex: `"The date today is " + date`
- Rather add parameter support to your messages and do something like:

```javascript
messages.date = "The date today is %date"... and then:msg( 'messages.date' );
```

#### What are `data-` attributes good for?

Data that should be associated with a particular element but need not have any defined meaning. Ex:

```html
<!-- HTML - Extra Info about “#electric-cars” -->
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

#### Consider HTML5 as an open web platform. What are the building blocks of HTML5?

- **Semantics**: allowing you to describe more precisely what your content is.
- **Connectivity**: allowing
  you to communicate with the server in new and innovative ways.
- **Offline Storage**: allowing
  webpages to store data on the client-side locally and operate offline more efficiently.
- **Multimedia**: making video and audio first-class citizens in the Open Web.
- **2D/3D Graphics and
  Effects**: allowing a much more diverse range of presentation options.
- **Performance and Integration**:
  providing greater speed optimization and better usage of computer hardware.
- **Device Access**: allowing for the usage of various input and output devices.
- **Styling**: letting authors write more
  sophisticated themes.

#### Describe the difference between a `cookie`, `sessionStorage` and `localStorage`?

- `localStorage`, `sessionStorage`, and `cookies` are all client storage solutions.
- **`localStorage`**: ...
- **`sessionStorage`**: ...
- **`cookies`**: ...

#### Describe the difference between `<script>`, `<script async>` and `<script defer>`?

- **`<script>`**: ...
- **`<script aync>`**: ...
- **`<script defer>`**: ...

#### Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?

- ...

#### What is progressive rendering?

- ...

#### Why you would use a `srcset` attribute in an image tag? Explain the process the browser uses when evaluating the content of this attribute?

- ...

#### Have you used different HTML templating languages before?

- ...

[Back to Contents](#Contents)

## [CSS](#CSS)

### Flexbox

### Grid

### Hierarchy & Inheritance

[Back to Contents](#Contents)

## [JavaScript](#JavaScript)

### Study Concepts

#### Explain event delegation

#### Explain how `this` works in JavaScript

#### Can you give an example of one of the ways that working with `this` has changed in ES6?

#### Explain how prototypal inheritance works

<!-- prettier-ignore -->
#### What's the difference between a variable that is: `null`, `undefined` or undeclared?

#### How would you go about checking for any of these states?

#### What is a closure, and how/why would you use one?

#### What language constructions do you use for iterating over object properties and array items?

#### Can you describe the main difference between the `Array.forEach()` loop and `Array.map()` methods and why you would pick one versus the other?

#### What's a typical use case for anonymous functions?

#### What's the difference between host objects and native objects?

#### Explain the difference between: `function Person(){}`, `var person = Person()`, and `var person = new Person()`?

#### Explain the differences on the usage of `foo` between `function foo() {}` and `var foo = function() {}`?

#### Can you explain what `Function.call` and `Function.apply` do? What's the notable difference between the two?

#### Explain `Function.prototype.bind`

#### What's the difference between feature detection, feature inference, and using the UA string?

#### Explain "hoisting"

#### Describe event bubbling

#### Describe event capturing

#### What's the difference between an "attribute" and a "property"?

#### What are the pros and cons of extending built-in JavaScript objects?

#### What is the difference between `==` and `===`?

#### Explain the same-origin policy with regards to JavaScript

#### Why is it called a Ternary operator, what does the word "Ternary" indicate?

#### What is strict mode? What are some of the advantages/disadvantages of using it?

#### What are some of the advantages/disadvantages of writing JavaScript code in a language that compiles to JavaScript?

#### What tools and techniques do you use debugging JavaScript code?

#### Explain the difference between mutable and immutable objects

- What is an example of an immutable object in JavaScript?
- What are the pros and cons of immutability?
- How can you achieve immutability in your own code?

#### Explain the difference between synchronous and asynchronous functions

#### What is event loop?

#### What is the difference between call stack and task queue?

#### What are the differences between variables created using `let`, `var` or `const`?

#### What are the differences between ES6 class and ES5 function constructors?

#### Can you offer a use case for the new arrow `=>` function syntax? How does this new syntax differ from other functions?

#### What advantage is there for using the arrow syntax for a method in a constructor?

#### What is the definition of a higher-order function?

#### Can you give an example for destructuring an object or an array?

#### Can you give an example of generating a string with ES6 Template Literals?

#### Can you give an example of a curry function and why this syntax offers an advantage?

#### What are the benefits of using `spread syntax` and how is it different from `rest syntax`?

#### How can you share code between files?

#### Why you might want to create static class members?

#### What is the difference between `while` and `do-while` loops in JavaScript?

[Back to Contents](#Contents)

## [Git](#Git)

### Study Concepts

[Back to Contents](#Contents)

## [CLI](#CLI)

### Study Concepts

[Back to Contents](#Contents)

## [Frameworks](#Frameworks)

### JS Frameworks

- ...

#### jQuery

- ...

#### React

- ...

#### Vue

- ...

#### Angular

- ...

#### Node

- ...

### CSS Libraries

- ...

#### Materialize

- ...

#### Skeleton

- ...

#### Bootstrap

- ...

### CSS Preprocessors

- ...

#### LESS

- ...

#### SASS/SCSS

- ...

[Back to Contents](#Contents)

## [Stacks](#Stacks)

- LAMP: Linux/Apache/MySQL/PHP
- MEAN: MongoDB/Express.js/AngularJS/Node.js
- MERN: MongoDB/Express.js/React/Node.js
- Ruby Stack: Ruby/Ruby on Rails/RVM (Ruby Virtual Machine)/MySQL/Apache/PHP
- Django Stack: Python/Django/Apache/MySQL
- Bitnami DevPack: PHP/Django/Ruby on Rails/Java/MySQL, PostgreSQL/Apache Tomcat

[Back to Contents](#Contents)

## [Fundamentals](#Fundamentals)

The following structure comes from [Teach Yourself Computer Science](https://teachyourselfcs.com/), and supplements the hands-on learning much of this guide focuses on with more rigorous study on core Computer Science topics. **You don't need to know formal CS to work in the tech industry**, but learning these concepts will give you a deeper understanding on the technologies and processes used in development.

### Programming

### Computer Architecture

### Algorithms & Data Structures

### Math for CS

### Operating Systems

### Computer Networking

### Databases

### Languages and Compiliers

### Distributed Systems

[Back to Contents](#Contents)

---

_To Do:_

- [ ] Test Build process for gh-pages deployment
- [ ] Create main page with checked/unchecked boxes to track progress
- [x] Create documentation layout
- [ ] Add sources for external reading, video, etc., for each pertinent section
- [ ] Split README into separate docs/wiki
- Add:
- [ ] Test Driven Development (TDD)
- [ ] Continuous Integration (CI)
- [ ] APIs
- [ ] [MDN Front End](https://developer.mozilla.org/en-US/docs/Learn/Front-end_web_developer)
  - Getting Started
    - [Installing basic software](<https://developer.mozilla.org/en-US/docs/Learn/> Getting_started_with_the_webInstalling_basic_software) — basic tool setup (15 min read)
    - [Background on the web and web standards](<https://developer.mozilla.org/en-US/docs/Learn/> Getting_started_with_the_webThe_web_and_web_standards) (45 min read)
    - [Learning and getting help](https://developer.mozilla.org/en-US/docs/Learn/Learning_and_getting_help) (45 min read)
    - Semantics and Structure with HTML
    - [Introduction to HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML) (15–20 hour readexercises)
    - [Multimedia and embedding](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding) (15–20 hour readexercises)
    - [HTML tables](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables) (5–10 hour read/exercises)
  - Styling and Layout with CSS
    - [CSS first steps](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps) (10–15 hour read/exercises)
    - [CSS building blocks](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks) (35–45 hour read/exercises)
    - [Styling text](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text) (15–20 hour read/exercises)
    - [CSS layout](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout) (30–40 hour read/exercises)
  - Interactivity with JavaScript
    - [JavaScript first steps](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps) (30–40 hour read/exercises)
    - [JavaScript building blocks](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks) (25–35 hour readexercises)
    - [Introducing JavaScript objects](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects) (25–35 hour readexercises)
    - [Client-side web APIs](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs) (30–40 hour readexercises)
    - [Asynchronous JavaScript](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous) (25–35 hour readexercises)
  - Web forms — Working with user data
    - [Web forms](https://developer.mozilla.org/en-US/docs/Learn/Forms) (40–50 hours)
  - Making the Web Work For Everyone
    - [Cross-browser testing](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Cross_browser_testing) (25–30hour read/exercises)
    - [Accessibility](https://developer.mozilla.org/en-US/docs/Learn/Accessibility) (20–25 hour read/exercises)
  - Modern Tooling
    - [Git and GitHub](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/GitHub) (5 hour read)
    - [Understanding client-side web development tools](<https://developer.mozilla.org/en-US/docs/Learn/> Tools_and_testingUnderstanding_client-side_tools) (20–25 hour read)
    - [Understanding client-side JavaScript frameworks](https://developer.mozilla.org/en-US/docs/Learn/ Tools_and_testingClient-side_JavaScript_frameworks) (30-60 hour read/exercises)\*
