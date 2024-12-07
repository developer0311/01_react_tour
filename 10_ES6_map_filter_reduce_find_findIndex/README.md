# **Array Methods in JavaScript**

JavaScript provides a variety of methods to manipulate and interact with arrays effectively. This document introduces five essential methods—`map()`, `filter()`, `reduce()`, `find()`, and `findIndex()`—with their descriptions, use cases, and examples.

---

## **1. Map**

The `map()` method creates a new array by applying a function to each element of the original array. It does not modify the original array but returns a transformed version.

### **Use Case**

- Transforming data into a new format or structure.

### **Example**

```javascript
const numbers = [3, 56, 2, 48, 5];
const squaredNumbers = numbers.map((num) => num * num);

console.log(squaredNumbers); // Output: [9, 3136, 4, 2304, 25]
```

---

## **2. Filter**

The `filter()` method creates a new array containing elements that pass a specified test (i.e., return `true` when a condition is applied).

### **Use Case**

- Extracting a subset of elements from an array.

### **Example**

```javascript
const numbers = [3, 56, 2, 48, 5];
const filteredNumbers = numbers.filter((num) => num > 10);

console.log(filteredNumbers); // Output: [56, 48]
```

---

## **3. Reduce**

The `reduce()` method applies a reducer function to each element in the array, resulting in a single accumulated value.

### **Use Case**

- Summing up numbers, calculating averages, or combining values.

### **Example**

```javascript
const numbers = [3, 56, 2, 48, 5];
const sum = numbers.reduce(
  (accumulator, currentValue) => accumulator + currentValue,
  0
);

console.log(sum); // Output: 114
```

---

## **4. Find**

The `find()` method returns the first element in an array that satisfies the specified condition. If no match is found, it returns `undefined`.

### **Use Case**

- Retrieving the first element that meets a particular criterion.

### **Example**

```javascript
const numbers = [3, 56, 2, 48, 5];
const firstLargeNumber = numbers.find((num) => num > 10);

console.log(firstLargeNumber); // Output: 56
```

---

## **5. FindIndex**

The `findIndex()` method returns the index of the first element in an array that satisfies a specified condition. If no element matches, it returns `-1`.

### **Use Case**

- Locating the position of the first matching element in an array.

### **Example**

```javascript
const numbers = [3, 56, 2, 48, 5];
const index = numbers.findIndex((num) => num > 10);

console.log(index); // Output: 1
```

---

### **Summary Table**

| **Method**        | **Action**                                                     | **Returns**                   |
| ----------------- | -------------------------------------------------------------- | ----------------------------- |
| **`map()`**       | Transforms elements in an array.                               | A new transformed array.      |
| **`filter()`**    | Filters elements based on a condition.                         | A new filtered array.         |
| **`reduce()`**    | Reduces the array to a single value using a function.          | A single accumulated value.   |
| **`find()`**      | Finds the first element that matches a condition.              | The first matching element.   |
| **`findIndex()`** | Finds the index of the first element that matches a condition. | The index of the first match. |

These array methods are versatile tools for handling and manipulating data in JavaScript applications, making your code cleaner and more efficient.
