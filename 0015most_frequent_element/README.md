# Most Frequent Element

### Problem

Write a function that finds the most frequent element in an array.

```
find_most_frequent_element([1, 2, 2, 3]) // 2
```

* **Prompt**: Does your approach work if two elements appear the same number of times, as in `[1, 2, 2, 3, 3]`?

In the example above (`[1, 2, 2, 3, 3]`), this loop would identify every element occurring twice: `2` and `3`.

### Hints

* Does your solution change if the input array is unsorted?

### Solutions

A complete solution should return all elements that occur `max` number of times, rather than just one of the most frequently occurring elements. For example, `find_most_frequent_element([1, 2, 2, 3, 3])` should return both `[2, 3]` as opposed to just `2` or `3`.

This solution runs in `O(n)` time with `O(n)` extra space.

- - -

### Copyright

Coding Boot Camp © 2016. All Rights Reserved.
