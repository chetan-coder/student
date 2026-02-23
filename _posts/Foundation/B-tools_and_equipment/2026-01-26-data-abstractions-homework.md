## Data Abstractions Homework

```js

    // HOMEWORK 1

    function calculator(num1, num2, operator) {
        let result;

        if (operator === "+") {
            result = num1 + num2;
        } else if (operator === "-") {
            result = num1 - num2;
        } else if (operator === "*") {
            result = num1 * num2;
        } else if (operator === "/") {
            result = num1 / num2;
        } else {
            result = "Invalid operator";
        }

        return result;
    }

    // HOMEWORK 2

    console.log(calculator(10, 5, "+"));
    console.log(calculator(10, 5, "-"));
    console.log(calculator(10, 5, "*"));
    console.log(calculator(10, 5, "/"));

    class Pet {
        eat() {
            console.log("Nom nom nom");
        }
    }

    class Dog extends Pet {
        bark() {
            console.log("Woof woof!");
        }
    }

    // Example usage
    const myDog = new Dog();
    myDog.eat();   // inherited from Pet
    myDog.bark();  // Dog's own method
