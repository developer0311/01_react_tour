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

```jsx
//Create a React app from scratch.
//Show a single h1 that says "Good morning" if between midnight and 12PM.
//or "Good Afternoon" if between 12PM and 6PM.
//or "Good evening" if between 6PM and midnight.
//Apply the "heading" style in the styles.css
//Dynamically change the color of the h1 using inline css styles.
//Morning = red, Afternoon = green, Night = blue.
```
