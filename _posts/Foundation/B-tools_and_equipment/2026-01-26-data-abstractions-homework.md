## Data Abstractions Homework

```js

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
