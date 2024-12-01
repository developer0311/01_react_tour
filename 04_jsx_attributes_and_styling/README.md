# **JSX Rules: Camel Casing and Self-Closing Tags**

JSX (JavaScript XML) extends JavaScript to allow HTML-like syntax in React components. However, JSX has some specific rules you must follow.

---

## **1. Camel Casing in JSX**

In JSX, attribute names use **camelCase** instead of hyphens, aligning with JavaScript conventions.

### Examples:

- Use `className` instead of `class`.
- Use `contentEditable` instead of `contenteditable`.
- Use `spellCheck` instead of `spellcheck`.

```jsx
<h1 className="title" contentEditable="true" spellCheck="false">
  Editable Heading
</h1>
```

---

## **2. Self-Closing Tags**

In JSX, all elements must be properly closed. Tags that do not require children must use a self-closing syntax `< />`.

### Examples:

- Correct:
  ```jsx
  <img src="image.jpg" alt="Example" />
  <br />
  ```
- Incorrect:
  ```jsx
  <img src="image.jpg" alt="Example">
  <br>
  ```

---

## **Example Code**

```jsx
import React from "react";
import ReactDOM from "react-dom";

ReactDOM.render(
  <div>
    <h1 className="heading" contentEditable="true" spellCheck="false">
      My Favourite Languages
    </h1>
    <ul>
      <li>Python</li>
      <li>Javascript</li>
      <li>C</li>
    </ul>
  </div>,
  document.getElementById("root")
);
```

## **Try it on CodeSandbox**

Check out the live example and experiment with the code on CodeSandbox:  
[Sandbox](https://codesandbox.io/p/sandbox/fervent-shirley-r67ggh)

