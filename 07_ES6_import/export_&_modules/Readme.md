# **ES6 Import/Export & Modules**

In JavaScript, **modules** allow you to break your code into reusable files. Using `import` and `export` syntax, you can share code between files while keeping your codebase clean and maintainable.  

## **Exporting from math.js**

The `math.js` file contains constants and functions that will be exported. Here's the code:  

```js
const pi = 3.1415962;

function doublePi() {
  return pi * 2;
}

function triplePi() {
  return pi * 3;
}

export default pi;
export { doublePi, triplePi };
```

---

## **Types of Imports**

### **1. Default Import**  
You can import the default export (`pi`) using any name you like.  

```js
import pi from "./math";
```

Example:  

```jsx
import React from "react";
import ReactDOM from "react-dom";
import pi from "./math";

ReactDOM.render(
  <ul>
    <li>{pi}</li>
  </ul>,
  document.getElementById("root")
);
```

---

### **2. Renamed Default Import**  
You can rename the default import to any other variable name.  

```js
import PI from "./math";
```

Example:  

```jsx
import React from "react";
import ReactDOM from "react-dom";
import PI from "./math";

ReactDOM.render(
  <ul>
    <li>{PI}</li>
  </ul>,
  document.getElementById("root")
);
```

---

### **3. Named Imports**  
You can import specific named exports, such as `doublePi` and `triplePi`.  

```js
import { doublePi, triplePi } from "./math";
```

Example:  

```jsx
import React from "react";
import ReactDOM from "react-dom";
import { doublePi, triplePi } from "./math";

ReactDOM.render(
  <ul>
    <li>{doublePi()}</li>
    <li>{triplePi()}</li>
  </ul>,
  document.getElementById("root")
);
```

---

### **4. Import All as an Object**  
You can import all exports as a single object and access them using dot notation.  

```js
import * as pi from "./math";
```

Example:  

```jsx
import React from "react";
import ReactDOM from "react-dom";
import * as pi from "./math";

ReactDOM.render(
  <ul>
    <li>{pi.default}</li>
    <li>{pi.doublePi()}</li>
    <li>{pi.triplePi()}</li>
  </ul>,
  document.getElementById("root")
);
```

---

### **5. Combined Default and Named Imports**  
You can combine importing the default export and specific named exports.  

```js
import PI, { doublePi, triplePi } from "./math";
```

Example:  

```jsx
import React from "react";
import ReactDOM from "react-dom";
import PI, { doublePi, triplePi } from "./math";

ReactDOM.render(
  <ul>
    <li>{PI}</li>
    <li>{doublePi()}</li>
    <li>{triplePi()}</li>
  </ul>,
  document.getElementById("root")
);
```

The `import` and `export` syntax makes JavaScript modular and efficient. Use default exports for single values and named exports for multiple utilities or constants. You can mix and match these as needed to keep your code clean and reusable.

---
## **Try it on CodeSandbox**

Check out the live example and experiment with the code on CodeSandbox:  
[Sandbox](https://codesandbox.io/p/sandbox/es6-import-export-modules-m2hf7p)