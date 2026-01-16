---
layout: post
title: Nested Conditionals with Coin Flip
permalink: /js/nestedconditionals
---

## Nested Conditionals – Coin Flip Example

This example shows how nested conditionals work using a coin flip.
The program decides who chooses first, then checks requirements using
if statements inside other if statements.

// Variables
let tickets = 20;
let height = 52;
let money = 10;
let itemInStock = true;

// Coin flip: 0 = heads, 1 = tails
let coinFlip = Math.floor(Math.random() * 2);

if (coinFlip === 0) {
    // Heads: you win the coin flip
    // You choose to do an activity

    if (tickets >= 15) {
        if (height >= 50) {
            // Result: You can do the activity
        } else {
            // Result: You are not tall enough
        }
    } else {
        // Result: Not enough tickets
    }

} else {
    // Tails: your friend wins the coin flip
    // Your friend chooses to buy something

    if (itemInStock === true) {
        if (money >= 8) {
            // Result: Item was purchased
        } else {
            // Result: Not enough money
        }
    } else {
        // Result: Item is out of stock
    }
}

// End of program