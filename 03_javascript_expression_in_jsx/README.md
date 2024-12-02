## JavaScript Expressions in JSX

In JSX, you can embed **JavaScript expressions** directly within your markup by enclosing them in curly braces `{}`. This feature makes JSX powerful and dynamic, enabling you to insert values, perform calculations, or call functions inside your UI components.

---

#### **What is a JavaScript Expression?**

A JavaScript expression is any valid unit of code that resolves to a value. Examples include variables, mathematical operations, function calls, and even ternary operators.

---

#### **Using JavaScript Expressions in JSX**

Here are some examples of how you can use JavaScript expressions in JSX:

1. **Embedding Variables**

   ```jsx
   const name = "John";
   const element = <h1>Hello, {name}!</h1>;
   // Output: Hello, John!
   ```

2. **Performing Calculations**
   ```jsx
   const price = 50;
   const tax = 0.1;
   const element = <p>Total: {price + price * tax}</p>;
   // Output: Total: 55
   ```
3. **React Sample**
   ```jsx
    import React from "react";
    import ReactDOM from "react-dom";

    const fName = "Diprati";
    const lName = "Das";
    const number = Math.floor(Math.random() * 10);

    ReactDOM.render(
    <div>
        <h1>Hello {`${fName} ${lName}`}!</h1> {/*ES6 Template Literals*/}
        <p>Your lucky number is: {number}</p>
    </div>,
    document.getElementById("root")
    );
    ```

---

#### **Important Notes**

- **Expressions Only:** JSX can handle expressions (e.g., `{1 + 1}`) but not statements like `if`, `for`, or `while`. For complex logic, move it outside JSX or use functions.
- **No Quotes Around Expressions:** Avoid wrapping expressions in quotes. For example:    

    ```jsx
    <p>{5 + 5}</p> // Correct
    <p>"{5 + 5}"</p> // Incorrect
    ```

---

#### **Sandbox Link**
- [Javascript Expressions In JSX](https://codesandbox.io/p/sandbox/javascript-expressions-in-jsx-xg3yw3)

---

By integrating JavaScript expressions, JSX allows you to create dynamic and interactive user interfaces efficiently! 🎉
