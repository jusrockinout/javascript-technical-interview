# Palindrome

### Problem

Write a function that determines if its string argument is a palindrome.

* **Prompt**: Is this the only solution?

### Hints

* Write down a palindrome. Can you point out which parts are equal?

  * **Follow-Up**. How would you check if those parts are equal?

* Can you think of a way to check if the front of the word is equal to the back of the word?

  * This is a fairly revealing hint. Only provide it if necessary.

### Solutions

#### Direct Solution

The simplest solution is simply to use the definition of a palindrome: If a string is equal to its reverse, return true. Otherwise, return false.

```
function palindrome (str) {
  if (str == str.split('').reverse().join(''))
    return true;
  else
    return false;
}
```

#### Array Solution

Another, less elegant, solution is to check that the first half of a string is equal to the reverse of the second half. In other words, `abba` is a palindrome because the first half, `ab`, is equal to the second half, `ba`, in _reverse_: `ab`.

#### Recursive Solution

A final solution is to check that the input string satisfies the basic property of a palindrome—that its first letter is equal to its last letter—and, if so, recursively check that the same is true for the substring that remains after removing the first and last letters.

- - -

### Copyright

Coding Boot Camp © 2016. All Rights Reserved.
