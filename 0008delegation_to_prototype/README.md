# Delegation to Prototype

## Problem

Consider the constructor function.

```
'use strict';

function User (firstName, lastName, email) {
  this.firstName = firstName;
  this.lastName = lastName;
  this.email = email;
}
```

1. How could you update this code such that all `User` objects have a `fullName` method that returns the user's full name? Sketch and implement your solution.

2. Can _all_ `User` objects call `fullName`—including those created _before_ you defined the method? If not, how would you update this code such that this is the case?

3. In your implementation, you use `User.prototype`. What object does `fullName` live on? Draw how it's related to individual `User` objects.

- - -

### Copyright

Coding Boot Camp © 2016. All Rights Reserved.
