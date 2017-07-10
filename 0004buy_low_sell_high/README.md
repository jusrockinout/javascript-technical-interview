# Buy Low Sell High

## Problem

Xena is an amateur day trader. Her portfolio consists of IAG. IAG is a mineral exploration company. Xena believes IAG has opportunity based on a gut feeling she has. Xena bought 10000 shares of IAG at $1.45 per share at 10 am on 12/12/15. She ended up selling it 20 minutes later at $1.74 making a $2900 profit. Xena just made 2 months of rent in 20 minutes.

These were all the prices of IAG on 12/12/15 during a one hour period in chronological order:

`$1.42, $1.32, $1.45, $1.20, $1.34, $1.74, $1.10, $1.89, $1.42, $1.90`

Write an efficient function that takes an array of stock prices in chronological order. The function should determine the largest profit possible during that period if someone bought the stock at the lowest price and sold it at the highest.

You must buy before you sell—no shorting.

* **Prompt**: What happens if the price _decreases_ all day?

      * The best candidates explain that they should `return` or `throw` (better) for arrays of length 1.

* **Prompt**: Is this the fastest solution?

### Hints

* Can we simply take the difference between the maximum and minimum elements?

  * We can't, because we can't guarantee that the maximum element occurs _after_ the minimum.

* Is it correct to loop through the entire array twice?

  * Not if the inner loop always starts at `0`.

  * Nested loops are correct only if the inner loop (with index `j`) starts at the index after that maintained by the outer loop (with index `i`).

* Can we loop through the array just once, and keep track of the maximum profit and minimum price we've seen _so far_?

  * **Follow-Up**. How do we know if we've found a new maximum profit?

  * **Follow-Up**. How do we know if we've found a new minimum price?

### Solutions

#### Brute Force | O(n^2)

The slow, brute force solution is to check every possible pair, and return the maximum. It is _correct_, but slow. It is, however, perfectly acceptable for candidates to start here.

#### Greedy Linear Search | O(n)

The best possible solution is to scan the array once, keeping track of the maximum profit identified so far and the minimum price.

- - -

### Copyright

Coding Boot Camp © 2017. All Rights Reserved.
