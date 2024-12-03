# **React Props**

### **Use Case of React Props**

React Props (short for properties) are used to pass data from one component to another in a React application. They make components reusable and dynamic by allowing customization via data inputs.

For example, a `Card` component can use props to render unique details like name, image, phone number, and email for different users.

---

### **React Props: Breaking Into Two Parts**

1. **Function Component (`Card`)**  
   The `Card` function represents a reusable component. It accepts `props` as an argument, allowing dynamic rendering of content passed from its parent.

   ```jsx
   function Card(props) {
     return (
       <div>
         <h2>{props.name}</h2>
         <img src={props.img} alt="avatar" />
         <p>{props.tel}</p>
         <p>{props.email}</p>
       </div>
     );
   }
   ```

   - **Why this part?**  
     The `Card` function defines the structure and how the passed data (props) is rendered. This is crucial for creating modular, reusable UI components.

2. **ReactDOM.render()**  
   This is the entry point where the parent component supplies props to the child `Card` component.

   ```jsx
   ReactDOM.render(
     <div>
       <Card
         name="John Doe"
         img="avatar.jpg"
         tel="123-456-7890"
         email="john.doe@example.com"
       />
     </div>,
     document.getElementById("root")
   );
   ```

   - **Why this part?**  
     It demonstrates how parent components (or ReactDOM) pass data to child components. This also reflects React's unidirectional data flow, ensuring that data flows from parent to child.

---

### **Difference Between HTML Attributes and React Props**

| **HTML Attribute**         | **React Props**            |
| -------------------------- | -------------------------- |
| Static and predefined.     | Dynamic and customizable.  |
| Used for native HTML tags. | Used for React components. |
| Follows HTML syntax.       | Follows JavaScript syntax. |

#### **Example: HTML Input Attribute**

```html
<input type="text" placeholder="Enter your name" />
```

- The `type` and `placeholder` are HTML attributes. They are static and cannot be passed dynamically as variables.

#### **Example: React Props**

```jsx
<Card
  name="Jane Doe"
  img="avatar2.jpg"
  tel="987-654-3210"
  email="jane.doe@example.com"
/>
```

- The `name`, `img`, `tel`, and `email` are props. They are passed dynamically from the parent and can be changed based on data.

---

React Props enable flexibility and modularity, making components highly reusable and adaptable in dynamic applications.

## **Try it on CodeSandbox**

Check out the live example and experiment with the code on CodeSandbox:  
[Sandbox](https://codesandbox.io/p/sandbox/react-props-fsd36v)
