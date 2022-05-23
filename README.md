# Frontend Mentor - Stats preview card component

![Design preview for the Stats preview card component coding challenge](./design/desktop-preview.jpg)

# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow


### What I learned

I had some issues with positioning the image, but then i remembered grid area :).

```css
.card-container {
        display: grid;
        grid-template-areas: 
        "t t i i"
        "t t i i";
        text-align: left;
        background: var(--clr-Dark-desaturated-blue);
        width: 63.25em;
        border-radius: 10px;
    }

    .hero-img {
        grid-area: i;
        background: url(./images/image-header-desktop.jpg) no-repeat;
        background-size: cover;
        background-position: center;
        background-color: var(--clr-Soft-violet);
        background-blend-mode: multiply;
        border-radius: 0 10px 10px 0;
        width: 450px;
        height: 55vh;
    }

    .card-content {
        grid-area: t;
        margin: 20px;
    }
```

