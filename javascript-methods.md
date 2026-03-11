<p align="center">
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="70"/>
</p>

# JavaScript Array Methods Cheat Sheet

JavaScript arrays provide many built-in methods that allow developers to transform, filter, search, and process data efficiently. These methods help simplify operations that would otherwise require loops and complex logic.

This cheat sheet highlights some commonly used JavaScript array methods with explanations and examples.

---

## map()

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="22"/>

The `map()` method creates a new array by applying a function to each element of the original array.

It does not modify the original array.

Example:

```javascript
const numbers = [1, 2, 3];

const doubled = numbers.map(n => n * 2);

console.log(doubled);
```

Output:

```
[2, 4, 6]
```

---

## filter()

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="22"/>

The `filter()` method creates a new array containing only the elements that satisfy a specified condition.

Example:

```javascript
const numbers = [1, 2, 3, 4];

const result = numbers.filter(n => n > 2);

console.log(result);
```

Output:

```
[3, 4]
```

---

## reduce()

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="22"/>

The `reduce()` method processes all elements in an array and reduces them to a single value.

It is commonly used for calculations such as totals or aggregations.

Example:

```javascript
const numbers = [1, 2, 3, 4];

const sum = numbers.reduce((total, n) => total + n, 0);

console.log(sum);
```

Output:

```
10
```

---

## find()

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="22"/>

The `find()` method returns the first element in an array that matches a specified condition.

If no element matches the condition, it returns `undefined`.

Example:

```javascript
const numbers = [1, 2, 3, 4];

const result = numbers.find(n => n > 2);

console.log(result);
```

Output:

```
3
```

---

## includes()

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="22"/>

The `includes()` method checks whether a specific value exists within an array.

It returns `true` if the value is found and `false` otherwise.

Example:

```javascript
const numbers = [1, 2, 3, 4];

console.log(numbers.includes(2));
```

Output:

```
true
```

---

## Summary

JavaScript array methods allow developers to manipulate data more efficiently without writing complex loops. Methods such as `map()`, `filter()`, and `reduce()` are especially useful in modern JavaScript development and functional programming patterns.
