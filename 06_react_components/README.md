# **React Components**

## **Why Components?**

Components are the building blocks of any React application. They make it easier to:

- **Reuse code**: Write once and use it multiple times.
- **Organize your project**: Break your UI into smaller, manageable pieces.
- **Enhance readability**: Each component handles a specific functionality, making the code easier to understand.

---

## **Folder Structure**

A typical folder structure for a React app using components looks like this:

```plaintext
src
│
├── components
|   │
|   ├── App.jsx        // Main component that renders other components
|   ├── Heading.jsx    // Component for the page heading
|   ├── List.jsx       // Component for the list items
|
├── index.js           // Entry point of the application
```

---

## **Component Code**

### **1. Heading.jsx**

This component renders a heading.

```jsx
import React from "react";

function Heading() {
  return <h1>My Favourite Languages</h1>;
}

export default Heading;
```

---

### **2. List.jsx**

This component renders a list of items.

```jsx
import React from "react";

function List() {
  return (
    <ul>
      <li>Python</li>
      <li>JavaScript</li>
      <li>C</li>
    </ul>
  );
}

export default List;
```

---

### **3. App.jsx**

This is the main component that combines `Heading` and `List`.

```jsx
import React from "react";
import Heading from "./Heading.jsx";
import List from "./List.jsx";

function App() {
  return (
    <div>
      <Heading />
      <List />
    </div>
  );
}

export default App;
```

---

### **4. index.js**

This is the entry point of the application, which renders the `App` component to the DOM.

```js
import React from "react";
import ReactDOM from "react-dom";
import App from "./components/App";

ReactDOM.render(<App />, document.getElementById("root"));
```

---

By structuring your app this way, each piece of functionality is encapsulated within its own component, making your React project modular, maintainable, and scalable.

## **Try it on CodeSandbox**

Check out the live example and experiment with the code on CodeSandbox:  
[Sandbox](https://codesandbox.io/p/sandbox/react-components-85nckw)
