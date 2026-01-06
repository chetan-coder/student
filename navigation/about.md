---
layout: post
title: About
permalink: /about/
comments: true
---

## As a Conversation Starter

Hi, my name is Chet. I am usually playing videogames, outside, or taking a nap.  
I moved here when I was 4. I started playing basketball when I was 5 and still continue playing it today.  
Another fact about me is that I have a sister who is 5 years old.

---

<style>
    /* GRID STYLES */
    .grid-container {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
        gap: 12px;
        margin-top: 15px;
    }

    .grid-item {
        padding: 10px;
        text-align: center;
        border-radius: 8px;
        border: 1px solid;
        background-color: #f9f9f9;
    }

    /* FORCE GRID TEXT TO BLACK (OVERRIDES THEME) */
    .grid-container .grid-item p {
        color: #000 !important;
    }

    .grid-item img {
        width: 100%;
        height: 120px;
        object-fit: cover;
        border-radius: 6px;
        margin-bottom: 6px;
    }

    /* IMAGE GALLERY */
    .image-gallery {
        display: flex;
        flex-wrap: nowrap;
        overflow-x: auto;
        gap: 10px;
        margin-top: 10px;
    }

    .image-gallery img {
        max-height: 150px;
        object-fit: cover;
        border-radius: 5px;
    }
</style>

---

## 🌍 Living in the World

<div class="grid-container" id="grid_container">
    <!-- Content added by JavaScript -->
</div>

<script>
    var container = document.getElementById("grid_container");
    var http_source = "https://upload.wikimedia.org/wikipedia/commons/";

    var living_in_the_world = [
        {"flag": "4/41/Flag_of_India.svg", "description": "Lived in India for 4 years"},
        {"flag": "f/f5/Flag_of_the_United_States_%281912-1959%29.svg", "description": "Lived in USA for 10 years"},
        {"flag": "d/d7/Washington_State_Flag.svg", "description": "Traveled to Washington - 2 times"},
        {"flag": "0/07/Flag_of_Dubai.svg", "description": "Traveled to Dubai - 4 times"}
    ];

    for (const location of living_in_the_world) {
        var gridItem = document.createElement("div");
        gridItem.className = "grid-item";

        var img = document.createElement("img");
        img.src = http_source + location.flag;

        var description = document.createElement("p");
        description.textContent = location.description;

        gridItem.appendChild(img);
        gridItem.appendChild(description);
        container.appendChild(gridItem);
    }
</script>

---

## 🎬 My Favorite Netflix Shows

<div class="grid-container" id="netflix_grid">
    <!-- Netflix grid items added by JavaScript -->
</div>

<script>
    const netflixContainer = document.getElementById("netflix_grid");

    const netflixShows = [
        { title: "Stranger Things", image: "{{site.baseurl}}/images/netflix/download (1).jpeg" },
        { title: "All American", image: "{{site.baseurl}}/images/netflix/download (2).jpeg" },
        { title: "Ninjago", image: "{{site.baseurl}}/images/netflix/ninjago.jpeg" },
        { title: "One Piece", image: "{{site.baseurl}}/images/netflix/download (1).jpeg" },
        { title: "Lost in Space", image: "{{site.baseurl}}/images/netflix/download (3).jpeg" }
    ];

    for (const show of netflixShows) {
        const item = document.createElement("div");
        item.className = "grid-item";

        const img = document.createElement("img");
        img.src = show.image;
        img.alt = show.title + " cover";

        const title = document.createElement("p");
        title.textContent = show.title;

        item.appendChild(img);
        item.appendChild(title);
        netflixContainer.appendChild(item);
    }
</script>

---

## 🏀 Journey Through Life

Here are some of the things I like to do in my free time:
- Basketball  
- Hang out with my friends  
- Play videogames with my friends  
- Watch TV shows  

---

## 👨‍👩‍👧 Culture, Family, and Fun

Everything for me, as for many others, revolves around family and faith.

- I was born in India and moved here when I was 4.
- I live with my mom, dad, and sister.
- Most of my family lives in India, and I usually visit them once a year.
- The gallery below shows some of the things I like to do in my free time.

<comment>
Gallery of pics showing things I enjoy
</comment>

<div class="image-gallery">
  <img src="{{site.baseurl}}/images/about/download.jpeg" alt="Gaming">
  <img src="{{site.baseurl}}/images/about/controllergame.jpg" alt="Controller">
  <img src="{{site.baseurl}}/images/about/bike2.png" alt="Bike">
  <img src="{{site.baseurl}}/images/about/park.jpg" alt="Park">
</div>
