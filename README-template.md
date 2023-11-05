# Frontend Mentor - Results summary component solution

This is a solution to the [Results summary component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/results-summary-component-CE_K6s0maV). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page
- **Bonus**: Use the local JSON data to dynamically populate the content

### Links

- Solution URL: [Add solution URL here](https://github.com/moaz890/results-summary)
- Live Site URL: [Add live site URL here](https://moaz890.github.io/results-summary/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

- Using Grid System with The Functions repeat() & minmax ()
- Using Flexbox With Both Directions Row & Column
- Using JSON Data File Using Fetch() function in JS


```js
fetch("data.json")
    .then((data) => data.json())
    .then((data) => {

      const items = document.querySelectorAll(".item");

      items.forEach((item, index) => {

        item.querySelector(".icon-small img").src = data[index].icon;
        item.querySelector(".title h5").innerText = data[index].category;
        item.querySelector(".score span").innerText = data[index].score;

      });

    });
```

### Continued development

- Animation 
- Grid System
- Powerful Layouts

## Author

- Frontend Mentor - [@moaz890](https://www.frontendmentor.io/profile/moaz890)
- Twitter - [@Prog_Abdelattey](https://www.twitter.com/Prog_Abdelattey)

