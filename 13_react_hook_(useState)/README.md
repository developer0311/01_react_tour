# **React Hooks: useState**

React introduced **Hooks** to let you use state and other React features in functional components (without writing a class).

The most common hook is **`useState`**, which lets you add and manage state in a component.

---

## **useState Basics**

- **Initial State**: You pass the starting value to `useState`.
- **Updater Function**: React gives you a function to update the state, which triggers a re-render.

**Syntax:**

```js
const [state, setState] = useState(initialValue);
```

---

## **Example: Showing Current Time**

```jsx
import React, { useState } from "react";

function Time() {
  const [time, setTime] = useState(new Date().toLocaleTimeString());

  function updateTime() {
    setTime(new Date().toLocaleTimeString());
  }

  return (
    <div>
      <h1>{time}</h1>
      <button onClick={updateTime}>Get Time</button>
    </div>
  );
}

export default Time;
```

---

✅ Here:

- `time` = state variable (holds current time).
- `setTime` = function to update state.
- Clicking the button updates and re-renders the new time.
