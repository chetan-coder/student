---
layout: post
title: Nested Conditionals with Coin Flip
permalink: /js/nestedconditionals
---

## Nested Conditionals Example (Numbers 1–50)

```js
// Loop through numbers 1 to 50
for (let num = 1; num <= 50; num++) {

    // First check: divisible by 1 (always true, but included for structure)
    if (num % 1 === 0) {

        // Nested check 1
        if (num % 2 === 0) {

            // Nested check 2
            if (num % 5 === 0) {

                // Nested check 3
                if (num % 10 === 0) {

                    // Nested check 4
                    if (num % 25 === 0) {

                        // Nested check 5
                        if (num % 50 === 0) {
                            console.log(num + " is divisible by all factors of 50 (1, 2, 5, 10, 25, 50)");
                        } else {
                            console.log(num + " is divisible by 1, 2, 5, 10, and 25");
                        }

                    } else {
                        console.log(num + " is divisible by 1, 2, 5, and 10");
                    }

                } else {
                    console.log(num + " is divisible by 1, 2, and 5");
                }

            } else {
                console.log(num + " is divisible by 1 and 2");
            }

        } else {
            console.log(num + " is divisible by 1 only");
        }
    }
}
