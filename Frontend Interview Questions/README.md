
# Frontend Developer Interview Questions

It includes topics of React.js, JavaScript, CSS, HTML, General Frontend Concepts.


## Author

- [Namit Kumar Singh](https://github.com/namitkumarsingh97)


## Here are some general tips and topics to focus on:

### Technical Topics:

1. **React.js:**

   - Understand React component lifecycle methods.
   - Explain the concept of state and props.
   - How does React handle forms and controlled components?
   - Know about React hooks (useState, useEffect, useContext, etc.).
   - Understand the virtual DOM and its significance.
   - Explain the differences between functional and class components.

2. **JavaScript:**

   - Know about ES6+ features (arrow functions, destructuring, spread/rest operators).
   - Understand closures and how they work.
   - Explain asynchronous JavaScript (Promises, async/await).
   - Be familiar with higher-order functions and callbacks.
   - Know how `this` works in different contexts.

3. **HTML and CSS:**

   - Understand the box model in CSS.
   - Know about CSS Flexbox and Grid layout.
   - Be familiar with responsive design principles.
   - Understand the semantic meaning of HTML tags.

4. **General Frontend Concepts:**
   - Cross-browser compatibility and testing.
   - Browser rendering process.
   - HTTP protocol and RESTful APIs.
   - Basic knowledge of version control systems (Git).

### Problem Solving and Coding:

1. **Algorithms and Data Structures:**

   - Be ready for coding challenges related to arrays, strings, and objects.
   - Understand common sorting and searching algorithms.
   - Solve problems on platforms like LeetCode or HackerRank.

2. **React Coding Challenges:**
   - Be prepared for challenges related to state management, component rendering, and lifecycle methods.
   - Practice writing clean and modular React code.

### Soft Skills and Communication:

1. **Project Experience:**

   - Be ready to discuss projects you've worked on, challenges faced, and how you overcame them.
   - Highlight any experience working in a team.

2. **Problem-Solving Approach:**

   - Communicate your thought process clearly when solving problems.
   - Break down complex problems into smaller, manageable steps.

3. **Ask Questions:**
   - Prepare a few thoughtful questions about the company, team, and projects.

### Additional Tips:

1. **Review Your Resume:**

   - Be ready to discuss your past experiences and projects in detail.

2. **Stay Calm:**

   - Take a deep breath and try to stay calm during the interview. It's okay to take a moment to think before answering.

3. **Online Presence:**
   - If you have any public code repositories or projects, make sure they are well-documented and showcase your skills.


## List of 100 technical interview questions covering React.js, JavaScript, HTML, CSS, and general frontend concepts:

### React.js:

#### 1. What is React and why is it used?

React is a JavaScript library for building user interfaces, particularly single-page applications where UI updates are frequent. It allows developers to create reusable UI components and efficiently manage the state of an application. React simplifies the process of updating the DOM by using a virtual DOM.

#### 2. Explain the concept of Virtual DOM in React.

The Virtual DOM is a lightweight copy of the actual DOM (Document Object Model). React uses it to optimize and speed up UI updates. When there is a change in the application state, React creates a virtual representation of the DOM, compares it with the previous one, and calculates the most efficient way to update the actual DOM, minimizing performance bottlenecks.

#### 3. What are the differences between class components and functional components?

* Class components use ES6 class syntax and extend from `React.Component`. They have a lifecycle and state management.
* Functional components are simpler and use function syntax. With the introduction of hooks in React, functional components can now also manage state and have lifecycle-like features.

#### 4. How do you handle state in React?

State in React is managed using the `useState` hook for functional components or `this.state` for class components. State can be updated using the provided setter function or `setState` method.

#### 5. Explain the significance of the `key` prop in React.

The `key` prop is used to uniquely identify elements in a list. It helps React efficiently update and reorder elements, minimizing unnecessary DOM manipulations and improving performance.

#### 6. What are React hooks? Provide examples of a few hooks.

React hooks are functions that allow functional components to use state and lifecycle features. Examples include:

* `useState` - for managing state,
* `useEffect` - for handling side effects,
* `useContext` - for accessing the context API,
* `useReducer` - for more complex state management.

#### 7. How does React Router work for navigation in a React application?

React Router is a library for handling navigation in React applications. It uses a declarative approach, allowing developers to define routes using components. The `<Route>` component renders UI based on the URL, and the `<Link>` component is used for navigating between different routes.

#### 8. Describe the purpose of the `useEffect` hook in React.

The `useEffect` hook is used for handling side effects in functional components. It can perform tasks like data fetching, subscriptions, or manually changing the DOM. It runs after the component renders and can clean up resources when the component is unmounted.

#### 9. What is prop drilling, and how can it be mitigated?

Prop drilling occurs when props are passed through multiple layers of components to reach a deeply nested child component. It can be mitigated by using context API to avoid passing props through intermediate components, making them directly accessible to deeply nested components.

#### 10. Differentiate between controlled and uncontrolled components in React.

* Controlled components: The component's state is controlled by React. Changes are handled using event handlers, and the state is managed via props.
* Uncontrolled components: The component's state is not controlled by React but by the DOM itself. The state is handled by the DOM, and React doesn't have direct control over it. `Refs` are often used to interact with uncontrolled components.

### JavaScript:

#### 11. Explain the event loop in JavaScript.

The event loop is a core concept in JavaScript that manages the execution of code. JavaScript is single-threaded, and the event loop enables asynchronous operations. It continuously checks the message queue for events (such as user interactions or timers), executes them one by one, and then returns to the loop.

#### 12. What is closure and how is it used in JavaScript?

A closure is the combination of a function and the lexical environment within which that function was declared. Closures allow a function to access variables from its outer (enclosing) scope even after that scope has finished executing. They are commonly used to create private variables, maintain state, and implement data encapsulation.

#### 13. Discuss the differences between `let`, `const`, and `var`.

`var`: Function-scoped, hoisted, can be redeclared and reassigned.
`let`: Block-scoped, hoisted, cannot be redeclared but can be reassigned.
`const`: Block-scoped, hoisted, cannot be redeclared or reassigned (immutable).

#### 14. How does asynchronous programming work in JavaScript?

Asynchronous programming in JavaScript is achieved through mechanisms like callbacks, promises, and async/await. It allows non-blocking execution of code, enabling tasks such as fetching data from a server, handling user input, and performing I/O operations without freezing the entire program.

#### 15. What is a Promise? How does it help in asynchronous programming?

A Promise is an object representing the eventual completion or failure of an asynchronous operation and its resulting value. It has states (`pending`, `fulfilled`, or `rejected`) and allows chaining callbacks to handle the asynchronous result. Promises improve the readability and maintainability of asynchronous code.

#### 16. Describe the differences between `null` and `undefined`.

* `null`: Represents the intentional absence of any object value. It is explicitly assigned.
* `undefined`: Represents the absence of a value in the variable, often the default value when a variable is declared but not assigned.

#### 17. Explain the concept of hoisting in JavaScript.

Hoisting is a JavaScript behavior where variable and function declarations are moved to the top of their containing scope during the compilation phase. This allows variables and functions to be used before they are declared in the code.

#### 18. How does `this` keyword work in different contexts in JavaScript?

`this` refers to the current execution context. Its value is determined by how a function is called:
In a regular function, `this` refers to the global object (e.g., `window` in a browser).
In a method (a function within an object), `this` refers to the object calling the method.
Using `call()`, `apply()`, or `bind()` allows explicit setting of `this`.
In arrow functions, `this` is lexically scoped, meaning it retains the value of `this` from its enclosing scope.

#### 19. What are arrow functions, and how do they differ from regular functions?

Arrow functions are a concise syntax for writing functions in JavaScript. They differ from regular functions in the following ways:

* No binding of `this`: Arrow functions inherit the `this` value from the enclosing scope.
* Cannot be used as constructors with `new`.
* No `arguments` object: Arrow functions do not have their own `arguments` object.

#### 20. What is the purpose of the `map` function in JavaScript?

The `map` function is used to transform each element of an array and create a new array with the results. It applies a provided function to each element, producing a new array of the same length. The original array remains unchanged. `map` is commonly used for iterating over arrays and performing operations on each element.

### HTML:

#### 21. What is the purpose of the `DOCTYPE` declaration in HTML?

The DOCTYPE declaration (`<!DOCTYPE html>`) specifies the HTML version being used and helps the browser render the web page correctly. It ensures that the browser uses the appropriate rendering mode, avoiding compatibility issues.

#### 22. Explain the semantic meaning of HTML5 tags like `<article>`, `<section>`, and `<nav>`.

`<article>`: Represents a self-contained piece of content that could be distributed and reused independently.
`<section>`: Defines a section in a document, typically with a heading, that groups together thematically related content.
`<nav>`: Represents a navigation menu or links to other pages or parts of the current page.

#### 23. How does HTML support responsive design?

HTML supports responsive design through the use of media queries and flexible layouts. Media queries allow CSS styles to be applied based on the characteristics of the device, such as screen width. Flexible layouts use relative units (like percentages) and fluid grids to adapt to different screen sizes.

#### 24. What is the purpose of the `meta` tag in HTML?

The `<meta>` tag is used to provide metadata about the HTML document. Common uses include specifying character encoding (`charset`), setting the viewport for responsive design (`viewport`), and providing descriptions for search engines (`description`, `keywords`).

#### 25. Describe the difference between `<div>` and `<span>` tags.

* `<div>`: A block-level element used to group other block-level or inline elements. It typically creates a new block-level box.
* `<span>`: An inline-level element used to apply styles or scripting to a specific portion of text or a small group of inline elements.

#### 26. What is the role of the `<head>` section in an HTML document?

The `<head>` section contains metadata about the HTML document, such as the title, links to stylesheets, scripts, and other meta-information. It is not directly visible on the webpage but plays a crucial role in defining the document's characteristics.

#### 27. How can you embed audio and video in HTML?

The `<audio>` and `<video>` elements are used to embed audio and video, respectively. They support various attributes like `src` (source), `controls` for playback controls, and others. Different formats (e.g., MP3, MP4) can be used depending on browser compatibility.

#### 28. What is the purpose of the `<canvas>` element in HTML5?

The `<canvas>` element provides a drawing surface for graphics using JavaScript. It allows dynamic rendering of graphics, charts, animations, and other visual elements. JavaScript is used to manipulate the content within the `<canvas>` element.

#### 29. Explain the difference between HTML and XHTML.

XHTML is a stricter and more XML-like version of HTML. It requires well-formed documents, follows XML rules, and has a stricter syntax. HTML is more forgiving and allows certain deviations from XML rules.

#### 30. How does HTML5 support offline web applications?

HTML5 introduces features like the Application Cache (`appcache`) and the Web Storage API. The Application Cache allows developers to specify files that should be cached for offline use, and the Web Storage API enables storing data locally on the user's device.

### CSS:

#### 31. Describe the box model in CSS.

The box model in CSS defines how elements are displayed in terms of content, padding, border, and margin. It consists of these layers, and their dimensions can be adjusted using CSS properties.

#### 32. Explain the difference between `margin` and `padding`.

* `Margin`: Clears space around the outside of an element. It contributes to the total space an element occupies but is outside the border.
* `Padding`: Clears space inside an element between the content and the border. It does not contribute to the total space the element occupies.

#### 33. How does CSS Flexbox work, and what are its advantages?

CSS Flexbox is a layout model that allows the design of a flexible and efficient layout structure. It provides a way to distribute space along a single axis (row or column) and supports alignment and order of items. Its advantages include simplified and more predictable layout structure, responsiveness, and ease of alignment.

#### 34. What is the purpose of the `z-index` property in CSS?

The `z-index` property determines the stacking order of positioned elements along the z-axis (depth). It is used to control the visibility and overlapping of elements on the page. Higher `z-index` values bring elements closer to the viewer.

#### 35. Discuss the differences between `display: inline` and `display: block`.

* `display: inline`: Elements are displayed inline, and only take up as much width as necessary. They do not start on a new line and cannot have top/bottom margins.
* `display: block`: Elements are displayed as block-level elements, starting on a new line and stretching the full width of the container. They can have top/bottom margins.

#### 36. How can you center an element horizontally and vertically in CSS?

Horizontal centering can be achieved using `margin: auto` or `text-align: center` on the parent container. Vertical centering can be achieved using techniques like flexbox (`align-items: center`) or positioning (`position: absolute` with `top: 50%; transform: translateY(-50%)`).

#### 37. Explain the CSS selector specificity.

Specificity is a measure of how specific a selector is in targeting HTML elements. It is represented by a four-part value, where each part contributes to the overall specificity. The more specific a selector, the higher its specificity.

#### 38. What is the purpose of the `box-sizing` property in CSS?

The `box-sizing` property controls how the total width and height of an element are calculated. The default value is `content-box`, which includes only the content. Setting it to `border-box` includes padding and border in the total width and height.

#### 39. Describe the difference between `position: relative`, `absolute`, and `fixed`.

* `position: relative`: Element is positioned relative to its normal position in the document flow.
* `position: absolute`: Element is positioned relative to its nearest positioned ancestor. If there is none, it is positioned relative to the initial containing block.
* `position: fixed`: Element is positioned relative to the browser window and will not move when the page is scrolled.

#### 40. How does CSS Grid layout work, and what are its advantages?

CSS Grid layout is a two-dimensional layout system for the web. It enables the creation of complex layouts with rows and columns. Its advantages include improved alignment, flexibility, and the ability to create responsive grid structures.

### General Frontend Concepts:

#### 41. What is responsive design, and how can it be achieved?

Responsive design is an approach to web design that makes web pages render well on a variety of devices and window or screen sizes. It involves using flexible grids and layouts, CSS media queries, and responsive images to adapt the content to different devices.

#### 42. Discuss the importance of cross-browser compatibility.

Cross-browser compatibility is crucial to ensure that a website or web application functions consistently across different web browsers. It prevents layout issues, broken features, and a poor user experience. Testing and adapting code to work with major browsers help maintain a consistent experience for all users.

#### 43. How does the browser rendering process work?

The browser rendering process involves multiple steps, including HTML parsing, constructing the Document Object Model (DOM), rendering tree creation, layout, painting, and composition. Each step contributes to rendering the web page and presenting it to the user.

#### 44. Explain the purpose of the Document Object Model (DOM).

The DOM is a programming interface for web documents. It represents the structure of a document as a tree of objects, where each object corresponds to a part of the document. The DOM allows scripting languages (e.g., JavaScript) to manipulate the content, structure, and style of a web page dynamically.

#### 45. Describe the differences between cookies and local storage.

Cookies are small pieces of data stored in the browser that persist across sessions and are sent with every HTTP request. They have a limited size and are used for client-server communication.

Local storage is a larger storage area (compared to cookies) that stores data on the client side. It persists even after the browser is closed and is commonly used for client-side data storage.

#### 46. What is the purpose of the HTTP protocol in web development?

HTTP (Hypertext Transfer Protocol) is the foundation of any data exchange on the web. It is used for communication between a client and a server. It defines how messages are formatted and transmitted, and it plays a key role in fetching resources, submitting forms, and more.

#### 47. Discuss the importance of optimizing website performance.

Optimizing website performance is crucial for providing a positive user experience. Faster-loading websites lead to higher user engagement, lower bounce rates, and improved search engine rankings. Techniques include minimizing HTTP requests, optimizing images, using efficient code, and implementing caching strategies.

#### 48. What is the purpose of a Content Delivery Network (CDN)?

A CDN is a network of servers distributed globally to deliver web content, such as images, stylesheets, and scripts, to users based on their geographical location. CDNs improve website performance by reducing latency, minimizing server load, and increasing content delivery speed.

#### 49. Explain the concept of Progressive Web Apps (PWAs).

PWAs are web applications that leverage modern web technologies to provide a native app-like experience. They can work offline, offer push notifications, and provide an immersive user experience. PWAs use service workers to enable offline functionality and caching.

#### 50. Describe the role of version control systems like Git in frontend development.

Version control systems, like Git, track changes to code over time. They allow developers to collaborate on projects, maintain a history of changes, and easily roll back to previous states. Git, in particular, is widely used for managing source code in frontend development, ensuring code integrity and collaboration.

### React.js:

#### 51. How does React handle forms and form validation?

React handles forms using controlled components, where form elements are controlled by React state. Form validation is often performed using state and event handlers to ensure data consistency. Conditional rendering can be used to display validation messages.

#### 52. Explain the concept of Higher Order Components (HOCs) in React.

Higher Order Components (HOCs) are functions that take a component and return a new component with enhanced functionality. They are a way to reuse component logic, share code, and add additional props or behavior to components.

#### 53. Discuss the differences between `class` and `className` in React.

In React, `class` refers to a JavaScript class (for defining components), while `className` is used to assign CSS classes to HTML elements. This differentiation helps avoid conflicts with the JavaScript `class` keyword.

#### 54. How can you optimize performance in a React application?

Performance optimization in React can be achieved through techniques such as:

* Memoization: Use of `React.memo` or `useMemo` to prevent unnecessary renders.
* Code splitting: Splitting large bundles into smaller chunks.
* Virtualization: Rendering only the visible elements in long lists.
* Proper component lifecycle methods usage.

#### 55. What is the purpose of the `shouldComponentUpdate` lifecycle method?

`shouldComponentUpdate` is a lifecycle method that allows optimization by deciding whether a component should re-render. If it returns `false`, the component will not update, preventing unnecessary rendering and improving performance.

#### 56. How does React handle events?

React uses synthetic events to normalize browser-specific event handling. Event handlers are camelCased (e.g., `onClick`) and attached to React elements. State updates triggered by events lead to re-renders, keeping the UI in sync with the application state.

#### 57. Explain the concept of React context and when it should be used.

React context provides a way to pass data through the component tree without having to pass props manually at every level. It should be used when data needs to be shared across multiple components, especially when dealing with deeply nested components.

#### 58. Discuss the significance of the `dangerouslySetInnerHTML` attribute in React.

`dangerouslySetInnerHTML` is used to insert HTML directly into a React component, but its use is discouraged due to potential security risks. It should only be used when the HTML content comes from a trusted source, as it can expose the application to cross-site scripting (XSS) attacks.

#### 59. How can you achieve code splitting in a React application?

Code splitting in React can be achieved using dynamic imports or tools like React's `lazy` and `Suspense`. This allows portions of the code to be loaded on-demand, reducing the initial bundle size and improving performance.

#### 60. Describe the role of error boundaries in React.

Error boundaries in React are components that catch JavaScript errors during rendering, in lifecycle methods, and during the handling of events. They allow developers to handle errors gracefully, preventing the entire application from crashing.

### JavaScript:

#### 61. Explain the concept of prototypal inheritance in JavaScript.

Prototypal inheritance is a mechanism where objects can inherit properties and methods from other objects through a prototype chain. Each object has a prototype object, and if a property or method is not found on the current object, JavaScript looks up the chain until it's found or reaches the end.

#### 62. Discuss the differences between `==` and `===` in JavaScript.

`==` (loose equality) compares values after type coercion, while `===` (strict equality) compares both values and types without coercion. `===` is generally recommended for avoiding unexpected type conversions.

#### 63. How can you clone an object in JavaScript?

Object cloning can be achieved using methods like `Object.assign({}, originalObject)` or the spread operator (`{ ...originalObject }`). It's important to note that these methods create a shallow copy, and nested objects may still reference the same objects.

#### 64. Explain the differences between `let` and `const`.

`let` allows the reassignment of variables, while `const` is used for constants and prevents reassignment after initialization. Both are block-scoped.

#### 65. What are the benefits of using `async/await` in JavaScript?

`async/await` is a syntax for handling asynchronous code, making it more readable and maintainable. It allows developers to write asynchronous code in a synchronous-like manner, improving error handling and avoiding callback hell.

#### 66. Discuss the concept of closures and their use cases.

Closures occur when a function is defined inside another function, allowing the inner function to access variables from the outer function's scope. They are used for encapsulation, data privacy, and creating factory functions.

#### 67. How can you handle errors in asynchronous JavaScript code?

Errors in asynchronous JavaScript code can be handled using `try/catch` blocks or by using the `.catch()` method on Promises. Additionally, `async/await` makes error handling more straightforward.

#### 68. What is the purpose of the `fetch` API in JavaScript?

The Fetch API is used for making HTTP requests in JavaScript. It provides a simpler and more powerful alternative to traditional XMLHttpRequest. It returns Promises and supports a cleaner syntax for handling responses.

#### 69. Explain the concept of promises and how they work.

Promises represent the eventual completion or failure of an asynchronous operation and its resulting value. They have three states: 
* `pending`
* `fulfilled`
* `rejected` 
Promises are used to handle asynchronous code more cleanly and avoid callback hell.

```javascript
let myPromise = new Promise(function(resolve, reject) {
// "Producing Code" (May take some time)

  resolve(); // when successful
  reject();  // when error
});

// "Consuming Code" (Must wait for a fulfilled Promise)
myPromise.then(
  function(value) { /* code if successful */ },
  function(error) { /* code if some error */ }
);
```

#### 70. Discuss the advantages of using ES6+ features in JavaScript.

ES6+ features bring improvements to JavaScript by introducing new syntax and functionalities. Some advantages include arrow functions, destructuring, template literals, classes, modules, and improved asynchronous programming with `async/await`.

### HTML:

#### 71. What is the purpose of the `<meta charset="UTF-8">` tag in HTML?

The `<meta charset="UTF-8">` tag specifies the character encoding for the HTML document. In this case, it indicates that the document should be interpreted as UTF-8, a character encoding that supports a wide range of characters and is commonly used for internationalization.

#### 72. How can you embed custom fonts in an HTML document?

Custom fonts can be embedded in an HTML document using the `@font-face` rule in CSS. This rule allows you to define a `font family`, link to the font file (e.g., TTF or WOFF), and apply the custom font to specific elements using the font-family property.

#### 73. Explain the use of the `<details>` and `<summary>` elements in HTML5.

The `<details>` and `<summary>` elements are used to create an interactive disclosure widget. The `<details>` element contains content that may be initially hidden, and the `<summary>` element provides a visible heading or label for the content. Users can click the summary to toggle the visibility of the content.

#### 74. Discuss the differences between the `<span>` and `<div>` elements.

* `<span>` and `<div>` are both container elements, but they are used in different contexts:
* `<span>` is an inline-level element and is often used for styling or scripting specific portions of text or inline content.
* `<div>` is a block-level element and is typically used as a container for larger sections of content, providing structure to the layout.

#### 75. What is the purpose of the `<noscript>` tag in HTML?

he `<noscript>` tag is used to provide alternative content that should be displayed when a browser does not support or has disabled JavaScript. It allows web developers to include content or instructions for users who have JavaScript disabled or unsupported.

#### 76. How does the `<script>` tag affect page loading in HTML?

The `<script>` tag is used to embed or reference JavaScript code in an HTML document. When placed in the `<head>` section without the `async` or `defer` attributes, it can block page rendering while the script is being fetched and executed. Using `async` or `defer` attributes allows the page to continue loading while the script is fetched and executed asynchronously.

#### 77. Explain the use of the `<time>` element in HTML5.

The `<time>` element in HTML5 is used to represent a specific period in time or a range of time. It can include a date, a time, or both. It helps machines understand and parse the content as a timestamp, providing semantic meaning to the displayed time information.

#### 78. How can you create a hyperlink that opens an email client in HTML?

To create a hyperlink that opens an email client, you can use the `<a>` (anchor) element with the `mailto`: scheme in the `href` attribute. For example: `<a href="mailto:email@example.com">Send Email</a>`. Clicking the link will open the default email client with the specified email address pre-filled.

#### 79. Describe the purpose of the `<aside>` element in HTML.

The `<aside>` element is used to define content that is tangentially related to the content around it. It is typically used for sidebars, pull quotes, advertisements, or other content that is not the main focus of the page but provides additional context or information.

#### 80. What is the role of the `<nav>` element in a webpage?

The `<nav>` element is used to define a navigation menu or links to other pages or parts of the current page. It is meant to encapsulate the primary navigation links of a webpage, providing semantic meaning to the navigation section. It helps assistive technologies and search engines understand the structure of the page.

### CSS:

#### 81. Discuss the advantages of using CSS preprocessors like Sass or Less.

CSS preprocessors, such as Sass or Less, offer several advantages:
* **Variables**: Allow for the definition and reuse of values throughout the stylesheet.
* **Nested Rules**: Enhance readability and structure by nesting selectors within each other.
* **Mixins**: Enable the reuse of blocks of styles across different selectors.
* **Functions**: Provide a way to create reusable pieces of code for dynamic styles.
* **Import**: Allow modularization by splitting styles into separate files.

#### 82. Explain the purpose of the `@media` rule in CSS.

The `@media` rule in CSS is used for media queries, allowing styles to be applied based on the characteristics of the device or viewport. It enables responsive design by specifying different styles for different screen sizes, resolutions, or other media features.

#### 83. How can you implement a sticky header in CSS?

To implement a sticky header in CSS, you can use the `position: sticky` property. Set the header's position to `sticky` and specify a `top` value to determine the point at which the header becomes sticky. For example:

```
header {
  position: sticky;
  top: 0;
  background-color: #ffffff;
}
```
#### 84. Discuss the differences between absolute and relative positioning in CSS.

* **Relative Positioning**: Positions an element relative to its normal position in the document flow. It can be moved using properties like `top`, `right`, `bottom`, or `left`, but it still occupies space in the document flow.
* **Absolute Positioning**: Positions an element relative to its nearest positioned ancestor (or the initial containing block if no positioned ancestor). It is taken out of the document flow and doesn't affect the positioning of other elements.

#### 85. How does the `transform` property work in CSS?

The `transform` property in CSS is used to apply 2D and 3D transformations to elements. It includes functions like `translate()`, `rotate()`, `scale()`, and more. Transformations are applied in the order specified, and they don't affect the layout of the document. Transforms can be animated using CSS transitions or animations.

#### 86. What is the purpose of the `currentColor` keyword in CSS?

The `currentColor` keyword in CSS is used to set the value of the `color` property to the computed value of the `color` property of the element itself. It is particularly useful when working with scalable vector graphics (SVG) or in cases where the color needs to be inherited from the surrounding context.

#### 87. Explain the concept of responsive images in CSS.

Responsive images in CSS involve using the `max-width` property to ensure that images do not exceed the width of their container. This helps prevent images from being too large on smaller screens. Additionally, the `width: 100%` rule is commonly used to make images responsive by making them fill the available width while maintaining their aspect ratio.

#### 88. How can you implement a CSS-only slider without JavaScript?

A CSS-only slider can be implemented using radio buttons and the `:checked` pseudo-class. Each radio button corresponds to a slide, and the `:checked` state is used to style the active slide. Transitions and animations can be applied to create sliding effects. This technique relies on the interaction between radio buttons and their associated labels.

#### 89. Discuss the benefits of using CSS frameworks like Bootstrap.

CSS frameworks like Bootstrap offer several benefits:
* **Rapid Development**: Provides a set of pre-designed components and styles, accelerating development.
* **Responsive Design**: Built-in responsiveness ensures compatibility with various screen sizes.
* **Consistency**: Maintains a consistent look and feel across the entire application.
* **Cross-browser Compatibility**: Frameworks are tested to work consistently across different browsers.
* **Customization**: Allows customization through theming and variable adjustments.

#### 90. How does the `rem` unit differ from the `em` unit in CSS?

Both **`rem`** and **`em`** are relative units in CSS:
* **`em`**: Represents the font size of the element, making it relative to the font size of its nearest parent or the element itself. If applied to non-text properties, it's relative to the font size of the element.
* **`rem`**: Stands for "root em" and is always relative to the font size of the root element (**`<html>`**). It ensures a consistent size regardless of the nesting level.

### General Frontend Concepts:

#### 91. What is lazy loading, and how can it improve website performance?

**Lazy loading**: Lazy loading is a technique that defers the loading of non-essential resources (such as images or scripts) until they are needed. This can significantly improve initial page load times by reducing the amount of data that needs to be loaded initially.

#### 92. Discuss the importance of SEO-friendly web development practices.

**SEO-friendly practices**: Implementing practices that make a website more accessible to search engines, such as:
* Proper use of semantic HTML.
* Descriptive and meaningful content.
* Optimized images with alt attributes.
* Clean and readable URL structures.
* Mobile-friendly and responsive design.

#### 93. Explain the role of the viewport meta tag in responsive design.

**Viewport meta tag**: In responsive design, the viewport meta tag (`<meta name="viewport" content="width=device-width, initial-scale=1.0">`) helps control the viewport's dimensions and scaling on different devices. It ensures that the page renders properly on various screen sizes and maintains a consistent user experience.

#### 94. How can you optimize images for the web?

**Image optimization**: Techniques to reduce image file sizes without sacrificing quality, including:
* Choosing the right file format (JPEG for photos, PNG for graphics with transparency, SVG for simple graphics).
* Compressing images using tools like ImageOptim or TinyPNG.
* Specifying image dimensions.
* Using responsive images with `srcset` attribute.

#### 95. Discuss the significance of ARIA roles in web accessibility.

**ARIA (Accessible Rich Internet Applications) roles**: A set of attributes that enhance the accessibility of web content for users with disabilities. ARIA roles define the roles of elements (e.g., buttons, landmarks) and their states, making web applications more navigable and understandable for screen readers and assistive technologies.

#### 96. What are web components, and how can they be used in frontend development?

**Web components**: A set of web platform APIs that allow the creation of reusable and encapsulated custom elements. They consist of four main technologies: Custom Elements, Shadow DOM, HTML Templates, and HTML Imports. Web components enable the creation of modular and reusable UI components.

#### 97. Explain the concept of critical rendering path in web performance.

**Critical rendering path**: The sequence of steps browsers take to convert HTML, CSS, and JavaScript into rendered pixels on the screen. Optimization of the critical rendering path involves minimizing render-blocking resources, optimizing CSS delivery, and deferring non-critical JavaScript to improve page load speed.

#### 98. How can you prevent common security vulnerabilities in web development?

**Security best practices**: Measures to prevent common vulnerabilities, including:
* Validating and sanitizing user inputs.
* Using HTTPS to encrypt data in transit.
* Implementing proper authentication and authorization.
* Regularly updating dependencies.
* Conducting security audits and penetration testing.

#### 99. Discuss the advantages and disadvantages of using a single-page application (SPA) architecture.

**SPA advantages**:
* Improved user experience with seamless navigation.
* Reduced server load due to client-side rendering.
* Efficient use of browser resources.
**SPA disadvantages**:
* Potentially slower initial load time.
* SEO challenges (although mitigated with techniques like server-side rendering).
* Complex client-side logic.

#### 100.  What is the purpose of a service worker in web development, and how does it relate to Progressive Web Apps (PWAs)?

**Service worker**: A script that runs in the background, separate from a web page, allowing features like offline support, push notifications, and background sync. In PWAs, service workers enhance the user experience by enabling offline functionality and improving performance by caching resources.