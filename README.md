# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

### The challenge

For this project I decided to force myself to use only SASS and specifically use, and in some cases over-use mixins as I wanted to get a feeling of what they are about in a smaller project.

### Screenshot

![](/public/images/product_preview_card_desktop.png)
![](/public/images/product_preview_card_mobile.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- Flexbox
- CSS Grid
- SASS with a focus on using mixins

### What I learned

I wanted to see if I could use a few mixins as 'template' for common actions like flexbox or formatting text. While I found it to be helpful in some cases I did discover that it ended up cluttering my CSS a little which ended up causing some issues towards the end of the project. I ended up needing to backtrack and either remove some rules or even overide things with media queries.

Also, I had some issues with gettin the image to work for me. For some reason those always trip me up. I started by applying the image as background-image so I could manipulate it to :cover but that ended up causing problems so I just linked it using <img src=""> and then applied object-fit which worked better.

To see how you can add code snippets, see below:

```css
@mixin flex($direction, $justify, $align, $display: flex) {
  display: $display;
  flex-direction: $direction;
  justify-content: $justify;
  align-items: $align;
}

@mixin text($family, $size, $weight, $color, $height, $spacing, $transform) {
  font-family: $family;
  font-size: $size;
  font-weight: $weight;
  color: $color;
  line-height: $height;
  letter-spacing: $spacing;
  text-transform: $transform;
}
```

### Continued development

A good lesson but still feel that I need to spend time understanding best practices for mixins as I feel like they will be incredibly advantageous.

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)
