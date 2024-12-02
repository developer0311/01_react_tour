# **Inline Styling in JSX**

It's very rare to use inline CSS, but if you really need it, here is the way to set inline CSS.

---

## **Format**

In JSX, inline styling is written as a **JavaScript object**. Since a JavaScript object is JavaScript code, we must wrap it in curly braces when injecting it into JSX.

```jsx
ReactDOM.render(
  <h1 style={{ color: "red" }}>Hello World!</h1>,
  document.getElementById("root")
);
```

- The **first curly braces** are for the JSX rule (to inject JavaScript).
- The **second curly braces** are for defining the JavaScript object.

---

## **Usage**

A good use of inline CSS is to create a variable for your styles. You can dynamically change the values as you would in any JavaScript object.

### **Example Code**

```jsx
import React from "react";
import ReactDOM from "react-dom";

const h1_style = {
  color: "red",
  fontSize: "50px",
};

// Dynamically change the style
h1_style.color = "blue";

ReactDOM.render(
  <h1 style={h1_style}>Hello World!</h1>,
  document.getElementById("root")
);
```

### **Try it on CodeSandbox**

Check out the live example and experiment with the code on CodeSandbox:  
[Sandbox](https://codesandbox.io/p/sandbox/inline-styling-in-jsx-8vwt8l)

---

## **React Styling Practice**

Strengthen your React skills with this styling exercise.

index.js:

```jsx
// Create a React app from scratch.
// Display a single <h1> with the following conditions:
// - Show "Good Morning" if the current time is between midnight (12:00 AM) and 12:00 PM.
// - Show "Good Afternoon" if the current time is between 12:00 PM and 6:00 PM.
// - Show "Good Evening" if the current time is between 6:00 PM and midnight (12:00 AM).
// Apply the "heading" style from styles.css to the <h1>.
// Dynamically change the color of the <h1> text using inline CSS based on the time of day:
// - Morning = red
// - Afternoon = green
// - Evening = blue
```

styles.css:

```css
.heading {
  font-size: 50px;
  font-weight: bold;
  border-bottom: 5px solid black;
}
```
