# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![](images/Screenshot.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- [Sass](https://sass-lang.com/) - For styles

### What I learned

Semantic tag for image exchange:

```html
  <picture>
        <source
          media="(max-width: 27.5rem)"
          srcset="images/image-product-mobile.jpg"
        />
        <img
          class="image"
          src="images/image-product-desktop.jpg"
          alt="Frasco de perfume, Gabrielle Essence."
        />
      </picture>
```
Use object-fit, so that the image is not aesthetic and loses quality:

```scss
.image {
    width: 100%;
    height: auto;
    border-radius: 0.7rem 0.7rem 0 0;
    display: block;
    object-fit: cover; // imagem não estica
  }
```
And use max-inline-size, so that the text only fits a certain amount of characters:

```scss
 p {
    line-height: 1.6;
    max-inline-size: 27ch;
  }
```

## Author

- Frontend Mentor - [@lucassalles-git](https://www.frontendmentor.io/profile/lucassalles-git)
- GitHub - [lucassalles-git](https://github.com/lucassalles-git)
