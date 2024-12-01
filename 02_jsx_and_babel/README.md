### Basic React Skeleton

```javascript
import React from "react";
import ReactDom from "react-dom";

// ReactDom.render(WHAT TO SHOW, WHERE TO SHOW IT)
// remember when we use the render method it can only take a single HTML element to render.
// we can wrap multiple elements in one to render them all
ReactDom.render(<h1>Hello World!</h1>, document.getElementById("root"));
```

---

### JSX
- **JSX (JavaScript XML)** is a syntax extension for JavaScript that allows you to write HTML-like code inside JavaScript.
- It makes React components easier to read and write by resembling HTML.
- Example:

  ```jsx
  const element = <h1>Hello, world!</h1>;
  ```
  Under the hood, JSX is converted to JavaScript using tools like Babel.

---

### Babel
- **Babel** is a JavaScript compiler that transforms modern JavaScript (including JSX) into code that browsers can understand.
- It ensures compatibility by converting ES6+ syntax and JSX into plain JavaScript.
- Try Babel -> https://babeljs.io/
- Example:

  ```jsx
  const element = <h1>Hello, world!</h1>;
  ```
  gets compiled to:

  ```javascript
  const element = React.createElement("h1", null, "Hello, world!");
  ```
