# The `map` & `parseInt` Puzzle

### Problem

Consider this line of JavaScript.

```
  ["1", "2", "3"].map(parseInt);
```

1. what do you expect this line of code to do? Explain your logic.

2. Run this snippet. What output do you get? Is this what you expected?

3. It's not immediately clear why we get this output. How would you go about figuring out what's wrong?

4. What would you search for if you could use Google?

5. Do you think you can explain what's going on?

      * In this case, we expect `map` to run `parseInt` on each string in the array, and convert them into integers.

        * In particular, we expect `["1", "2", "3"].map(parseInt)` to output `[1, 2, 3]`.

        * But instead, that is incorrect. Why?

- - -

### Copyright

Coding Boot Camp © 2016. All Rights Reserved.
