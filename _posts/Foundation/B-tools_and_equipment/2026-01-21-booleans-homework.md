## Booleans Homework

```js

    function isPositiveAndOdd(num) {
        let isPositive = num > 0;
        let isOdd = num % 2 === 1;
        return isPositive && isOdd;
    }

    console.log(isPositiveAndOdd(11)); // false

// Tested in Code Runner and it works