# Curried Sum

## Problem

Write a function that adds two numbers, and can be called either of two ways:

```
sum(2, 3); // 5
sum(2)(3); // 5
```
Implement solution only after you have explained at least the first three prompts-in particular, until you articulate the following points:

1. `sum` either returns a result immediately, or returns a function;
2. `sum` decides which of these to do by checking if it got two arguments, as in `sum(2, 3)`, or one argument, as in `sum(2)`.
3. When we call it like `sum(2)`, `sum` returns a function that "remembers" the `2`.

* **Prompt**: Can you explain what this function does if we pass two arguments "normally"? That is, if we call it like `sum(2, 3)`?

* **Prompt**: Can you explain what's happening if we pass arguments the second way? that is, if we call it like `sum(2)(3)`?

  * **Hints**

    * Imagine we could do: `var y = sum(2)`. Then, `sum(2)(3)` is the same as `y(3)`. What's happening when we write `y(3)`?

      * The correct response is: We're calling `y` as a function.

      * **Follow-Up**. If we're calling `y` as a function, and `y = sum92)`, what does `sum(2)` do?

* **Prompt**: How does `sum` know whether to return a result immediately—as in `sum(2, 3)`—or to return a function—as with `sum(2)`?

* **Prompt**: How would you pseudo-code a solution?

    * **Sketches Conceptual Solution**. Pseudo-code that solves the problem at a high level. It would look something like:


```
function sum first_numner, second_number
  if (sum received two arguments)
    return first_number + second_number
  else if (sum received one argument)
    return function that takes a second number, and adds it to the first_number
```

- - -

### Copyright

Coding Boot Camp © 2016. All Rights Reserved.
