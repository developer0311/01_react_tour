# **Ternary Operator in JavaScript vs React**

## **Introduction**

The **ternary operator (`?:`)** in JavaScript is a shorthand way to write conditional expressions. It allows you to return one value if a condition is `true` and another if it is `false`.

In **React**, the ternary operator and logical `&&` are commonly used for **conditional rendering** of components and elements.

---

## **Ternary Operator (`?:`) in JavaScript**

The ternary operator works as a compact alternative to `if...else`.
**Syntax:**

```js
condition ? expressionIfTrue : expressionIfFalse;
```

**Example (JavaScript):**

```js
const age = 18;
const message = age >= 18 ? "You are an adult." : "You are a minor.";
console.log(message); // Output: You are an adult.
```

---

## **Ternary Operator (`?:`) in React**

In React, ternary operators are often used for **conditional rendering** inside JSX.

**Example (React):**

```jsx
function App() {
  const currentTime = 14;

  return (
    <div>
      {currentTime > 12 ? (
        <h1>Why are you still working?</h1>
      ) : (
        <h1>Good Morning!</h1>
      )}
    </div>
  );
}
```

Here:

- If `currentTime > 12`, React renders **"Why are you still working?"**
- Otherwise, it renders **"Good Morning!"**

---

## **Logical AND (`&&`) in React**

Sometimes you only want to render something if a condition is `true`. Instead of using a ternary with `null`, you can use the **`&&` operator**.

**Example (React):**

```jsx
function App() {
  const currentTime = 14;

  return <div>{currentTime > 12 && <h1>Why are you still working?</h1>}</div>;
}
```

Here:

- If `currentTime > 12`, the `<h1>` will render.
- If the condition is `false`, React renders **nothing**.

---

## **Difference Between `?:` and `&&` in React**

- Use **`?:`** when you want to render **one thing or another** (two possible outcomes).
- Use **`&&`** when you want to render something **only if a condition is true**, otherwise render nothing.

---

✅ **Tip:**

- `?:` → Great for "either/or" conditions.
- `&&` → Great for "only if true" conditions.
