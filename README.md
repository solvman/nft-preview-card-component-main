# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](./screenshot.jpg)

### Links

- Solution URL: [https://github.com/solvman/nft-preview-card-component-main](https://github.com/solvman/nft-preview-card-component-main)
- Live Site URL: [https://glittering-churros-e02ae5.netlify.app/](https://glittering-churros-e02ae5.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

It was pretty interesting to learn how to do hover effect on an image with an icon overlay:

```html
<div class="card__img">
  <img
    src="./images/image-equilibrium.jpg"
    alt="glass cube on dark background"
  />
  <div class="card__img__overlay"></div>
  <img
    class="card__img__overlay__icon"
    src="./images/icon-view.svg"
    alt="icon view"
  />
</div>
```

```css
.card__img {
  position: relative;
  border-radius: 8px;
  margin-bottom: 24px;
  overflow: hidden;
  cursor: pointer;
}

.card__img:hover .card__img__overlay {
  opacity: 0.5;
}

.card__img:hover .card__img__overlay__icon {
  opacity: 1;
}

.card__img__overlay {
  background-color: var(--clr-primary-cyan);
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  opacity: 0;
  position: absolute;
  transition: 0.5s ease;
}

.card__img__overlay__icon {
  position: absolute;
  top: 50%;
  left: 50%;
  opacity: 0;
  transform: translate(-50%, -50%);
}
```

## Author

- Website - [Github](https://github.com/solvman)
- Frontend Mentor - [@solvman](https://www.frontendmentor.io/profile/solvman)
- Twitter - [@leofitz1111](https://twitter.com/leofitz1111)
