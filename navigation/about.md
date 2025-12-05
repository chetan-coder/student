---
layout: post
title: About
permalink: /about/
comments: true
---

## As a conversation Starter

Hi, my name is Chet. I am usually playing videogames, outside, or taking a nap. I also mvoed here when I was 4. I started playing basketball when I was 5, and still continue playing it today. Another fact about me is that I have a sister that is 5.

<style>
    /* Style looks pretty compact, 
       - grid-container and grid-item are referenced the code 
    */
    .grid-container {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(150px, 1fr)); /* Dynamic columns */
        gap: 10px;
    }
    .grid-item {
        text-align: center;
    }
    .grid-item img {
        width: 100%;
        height: 100px; /* Fixed height for uniformity */
        object-fit: contain; /* Ensure the image fits within the fixed height */
    }
    .grid-item p {
        margin: 5px 0; /* Add some margin for spacing */
    }

    .image-gallery {
        display: flex;
        flex-wrap: nowrap;
        overflow-x: auto;
        gap: 10px;
        }

    .image-gallery img {
        max-height: 150px;
        object-fit: cover;
        border-radius: 5px;
    }
</style>

<!-- This grid_container class is used by CSS styling and the id is used by JavaScript connection -->
<div class="grid-container" id="grid_container">
    <!-- content will be added here by JavaScript -->
</div>

<script>
    // 1. Make a connection to the HTML container defined in the HTML div
    var container = document.getElementById("grid_container"); // This container connects to the HTML div

    

    // 3a. Consider how to update style count for size of container
    // The grid-template-columns has been defined as dynamic with auto-fill and minmax

    // 3b. Build grid items inside of our container for each row of data
    for (const location of living_in_the_world) {
        // Create a "div" with "class grid-item" for each row
        var gridItem = document.createElement("div");
        gridItem.className = "grid-item";  // This class name connects the gridItem to the CSS style elements
        // Add "img" HTML tag for the flag
        var img = document.createElement("img");
        img.src = http_source + location.flag; // concatenate the source and flag
        img.alt = location.flag + " Flag"; // add alt text for accessibility

        // Add "p" HTML tag for the description
        var description = document.createElement("p");
        description.textContent = location.description; // extract the description

        // Add "p" HTML tag for the greeting
        var greeting = document.createElement("p");
        greeting.textContent = location.greeting;  // extract the greeting

        // Append img and p HTML tags to the grid item DIV
        gridItem.appendChild(img);
        gridItem.appendChild(description);
        gridItem.appendChild(greeting);

        // Append the grid item DIV to the container DIV
        container.appendChild(gridItem);
    }
</script>

### Journey through Life

Here are some of the stuff I like to do in my free time

- Basketball
- Hang out with my friends
- Play videogames with my friends
- Watch TV Shows

### Culture, Family, and Fun

Everything for me, as for many others, revolves around family and faith.

- I was born in India, and mmove here when I was 4.
- I live with my Mom, Dad, and sister here. While, the rest of my family lives in India. I usually visit them once a year.
- The gallery of pics shows some of the things that I usually do in my free time

<comment>
Gallery of Pics, I like to do in my free time
</comment>
<div class="image-gallery">
  <img src="{{site.baseurl}}/images/about/download.jpeg" alt="Image 1">
  <img src="{{site.baseurl}}/images/about/controllergame.jpg" alt="Image 2">
  <img src="{{site.baseurl}}/images/about/bike2.png" alt="Image 3">
  <img src="{{site.baseurl}}/images/about/park.jpg" alt="Image 4">
</div>
