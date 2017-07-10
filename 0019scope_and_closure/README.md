# Scope & Closure

### Problem

Consider the snippet below.

```
var obj = {};

function foo () {
  var updated = 0;

  return bar;
}

function bar (arg) {
  var key = JSON.stringify(arg);

  if (!(obj[key])) {
    obj[key] = arg
  }
  else {
    return obj[key];
  }

  console.log(updated);
}
```

1. What will happen if we call `bar`? Why? How can we rearrange our code to fix this, and why does this work?

2. After updatin your code, explain where `bar` and `obj` are visible, and why.

3. Run `foo`; store its return value in a variable; and experiment with it. Explain its behavior. What fundamental JavaScript concept is responsible for this behavior?


This problem tests knowledge of **scope** and **closure**.

* **Prompt**: How can we modify this code so that `bar` is only visible in `foo`?

* **Prompt**: When we run `foo`, what does it return?

* **Prompt**: When we execute the return value of `foo`, what does it do?

- - -

### Copyright

Coding Boot Camp © 2016. All Rights Reserved.
