---
layout: post
title: Array Homework Excercies 1-3
permalink: /js/arrays
---

## Excercie 1

let food = ["watermelon", "orange", "juice", "fries", "burger"];

console.log("My array of food:");
console.log(food);
console.log();

console.log("First fruit (index 0):", food[0]);
console.log("Third fruit (index 5):", food[5]);
console.log();

cd
console.log("Number of food:", food.length);


## Excerice 2

let shoppingList = ["milk", "bread", "eggs", "apples"];

console.log("My shopping list:");
console.log(shoppingList);
console.log();

console.log("First item (index 0):", shoppingList[0]);
console.log("Third item (index 2):", shoppingList[2]);
console.log();

console.log("Number of items:", shoppingList.length);

## Excercise 3

let numbers = [1, 2, 3, 4, 5];
let sum = 0;

for (let i = 0; i < numbers.length; i++) {
    console.log(numbers[i]);
    console.log(numbers[i] * 2);
    sum = sum + numbers[i];
}

console.log("Sum:", sum);
