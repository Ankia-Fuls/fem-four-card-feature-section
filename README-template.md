# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![The screenshot of the completed design](./design/Screenshot%20Completed%20Frontend%20Mentor%20Four%20card%20feature%20section.png)

### Links

- Solution URL: [GitHub Repository](https://github.com/Ankia-Fuls/fem-four-card-feature-section)
- Live Site URL: [GitHub Pages](https://ankia-fuls.github.io/fem-four-card-feature-section/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid
- Mobile-first workflow
- SASS Styling and functions

### What I learned

I learned how to use the css box-shadow property to give a slight border effect to the cards. I also learned how to use the :before selector to customize the colored bars at the top of the cards. I created a mixin with SASS to avoid repeating most of the code that would be needed for each :before element and to just replace the color as shown below.

```css
@mixin color-bar ($color) {
    content: "";
    display: block;
    width: 100%;
    height: rem(5);
    background-color: $color;
    position: absolute;
    left: 0;
    top: 0;
}
```
This code created the 5px wide color bars at the top of each card by using the code as shown below.

```css
.team:before {
        @include color-bar($red);
    }
```

### Continued development

I would like to play around more with box-shadow and the different effects that can be obtained by using it. I would also like to come back to the project at one point to add accessibility to the project since I did not take it into account for this project.

### Useful resources

- [Box Shadow Styling](https://css-tricks.com/almanac/properties/b/box-shadow/) - This helped me with understanding how box-shadow worked and how to get the effect I wanted.
- [Grid Area](https://www.w3schools.com/cssref/pr_grid-area.php) - This helped me to define how the different cards were placed within my grid.

## Author

- Frontend Mentor - [@Ankia-Fuls](https://www.frontendmentor.io/profile/Ankia-Fuls)
- GitHub - [@Ankia-Fuls](https://github.com/Ankia-Fuls)
