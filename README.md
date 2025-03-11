# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Frontend Mentor - Testimonials grid section solution](#frontend-mentor---testimonials-grid-section-solution)
  - [Table of contents](#table-of-contents)
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

![Macbook](screenshots/Macbook-Air-1559x975.png)

![iPhone14](screenshots/iPhone-14-Pro-393x2176.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- [SASS](https://sass-lang.com/documentation/) - SASS library

### What I learned

One of the things i learned specially was how we structure everything that has to do with `Sass`like:

- How to import styles from different assets

```scss
@use "colors";
@use "reset";
@use "base";
@use "card__layout";
@use "card";
@use "media__query";
```

- How to create `mixins`

```scss
@mixin square($size, $radius: 0) {
  width: $size;
  height: $size;

  @if $radius != 0 {
    border-radius: $radius;
  }
}
```

- I learned too a way to style divs and change his order

```css
.card:nth-child(1) {
  grid-column: 1/3;
}
.card:nth-child(3) {
  grid-column: 1/2;
  grid-row: 2/3;
}
.card:nth-child(4) {
  grid-column: 2/4;
}
.card:nth-child(5) {
  grid-column: 4/5;
  grid-row: 1/3;
}
```

### Continued development

I want to keep learning about `SASS`because it is very simple to work with

### Useful resources

- [Midudev](https://www.youtube.com/watch?v=iTjkiI8QQsM&ab_channel=midulive) - Here i learned how to build the grid

## Author

- Frontend Mentor - [@ekondongayecaba](https://www.frontendmentor.io/profile/EkoNdongAyecaba)
- Twitter - [@EkoNdongAyecaba](https://x.com/Shiitake_EGBM)
