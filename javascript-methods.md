# JavaScript Array Methods Cheat Sheet

JavaScript arrays provide several built-in methods to manipulate data.

## map()

Creates a new array by applying a function to each element.

Example

const numbers = [1,2,3]
numbers.map(n => n * 2)

---

## filter()

Returns elements that satisfy a condition.

Example

numbers.filter(n => n > 1)

---

## reduce()

Reduces array to a single value.

Example

numbers.reduce((sum, n) => sum + n, 0)

---

## find()

Returns the first element matching a condition.

numbers.find(n => n > 2)

---

## includes()

Checks if an element exists in array.

numbers.includes(2)
