# Global var

### Problem

Consider the following snippet of JavaScript.

```
for (var i = 0; i < 5; i += 1) {
  setTimeout(function () {
      console.log(i);
    }, i * 1000);
}
```

1. What do you expect this code to do?

2. What will this log, and why?

3. How can you "fix" this code, if you expected it to behave differently than it did?

### Hints

* What is the value of `i` when the callbacks to `setTimeout` run?

### Solutions

#### Use `let`

#### IIFE

The classical solution uses an IIFE to bind the value of `i` on each iteration to each callback's closure.

- - -

### Copyright

Coding Boot Camp © 2016. All Rights Reserved.
