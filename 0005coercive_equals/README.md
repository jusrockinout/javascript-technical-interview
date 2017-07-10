# Coercive Equals

## Problem

This multi-part problem drills a candidate's familiarity with JavaScript.

1. What is the difference between `==` and `===`?

2. What are the advantages to using `==`? To using `===`?

3. When might we prefer the one over the other?

### Prompts

* **Prompt**: What is the difference between `==` and `===`?

  * **Look For**

      * The `===` returns true only if the items being compared have the same value _and_ type. The `==` returns true if the items being compared have the same value, even if they don't have the same type.

      * The `==` is _coercive_—it tries to force the items being compared to be equal, and returns `true` if it can, but `false` if it can't. The `===` is _strict_—it only returns true if the items being compared have the same value and type.

    * **Hints**.

      * Does `1 == "1"` evaluate to `true` or `false`? What about `1 === 1`? What do `1` and `"1"` have in common? What's different?

* **Prompt**: Can you think of any advantages to using `==` over `===`, and vice versa?

      * One advantage to using `===` is that it only ever returns `true` when both items being compared are, in fact, strictly equal—informally, it always does what we expect: `[] === 0` is `false`.

        * This is an advantage uniue to `===`, as `==` returns `true` for items that are _coercivel_ equal/which can be _forced_ to be equal. For example, `[] == 0` is `true`.

* **Prompt**: When might we prefer one over the other?

      * Some candidates might suggest that we might prefer `==` when checking equality to `undefined`, as in `if (x == null)`. This is also legitimate—the alternative with `===` is longer and arguably less readable: `if (x === null && x === undefined)`.

- - -

### Copyright

Coding Boot Camp © 2016. All Rights Reserved.
