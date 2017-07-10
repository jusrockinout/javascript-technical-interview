# Array Deep Equals

## Problem

Suppose you have two arrays with the same contents.

```
var first = [1, 2, 3];
var second = [1, 2, 3];
```

1. What happens when you test if these arrays are equal using `==`? Using `===`? Is this what you expect?

2. Write a function that tests if the contents of two arrays are equal.

When you compare two arrays with `==` or `===`, as in `first === second`, JavaScript checks if `first` refers to the _same array_ as `second`—it does **not** check if `first` contains the same elements.

The test in this snippet evaluates to true:

```
// first and second refer to the same array...
var first = second = [1, 2, 3];

// ...So they test equal!
first === second; // true
```

...But if we want to compare the _contents_ of two arrays, we have to write our own function to do so.

* **Prompt**: Can you explain why `first === second` returns false?

      * Candidates should be able to explain that a properly implemented function will return `true` if every element in the two arrays is equal, and `false` otherwise.

### Notes

Strong candidates will note that even some solutions that properly handle nested arrays and objects will fail for nested arrays that contain equal elements but in different orders. For example:

```
var first = [1, 2, 3];
var second = [2, 1, 3];

deepEquals(first, second); // false
```
- - -

### Copyright

Coding Boot Camp © 2016. All Rights Reserved.
