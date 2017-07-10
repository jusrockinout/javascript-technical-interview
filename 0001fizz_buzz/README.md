# "FizzBuzz"

## Problem

Write a script that prints the numbers 1 to 100 in the console. But for multiples of three, print `Fizz` instead of the number. For multiples of five, print `Buzz`. For numbers which are multiples of both three and five, print `FizzBuzz`.

### Hints

* Does the order in which we check if our number is a multiple of 3, 5, or both matter?

### Solution

#### Brute Force | Constant Time

The solution is simply to check that the current number is a multiple of both 3 and 5; and then check whether it is a multiple of 3 or 5 if it is not.

```
var fizzBuzz = function(){

  // Loop 100 times, starting from the number 1
  for(var i = 1; i <= 100; i++){

    // If divisible by 3 and 5
    if(i % 3 === 0 && i % 5 === 0) {
      console.log('FizzBuzz');

    } 
    // If divisible by 3
    else if (i % 3 === 0) {
      console.log('Fizz');

    } 
    // If divisible by 5
    else if (i % 5 === 0) {
      console.log('Buzz');

    } 
    // If not divisible either 3 or 5
    else {
      console.log(i);
    }
  }
};
```

- - -

### Copyright

Coding Boot Camp © 2016. All Rights Reserved.
