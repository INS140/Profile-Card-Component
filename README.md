# Frontend Mentor - Profile card component

![Design preview for the Profile card component coding challenge](./design/desktop-preview.jpg)

## Table of contents

- [Overview](#overview)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

This is another challenge from the Frontend Mentor website that I have completed. I chose this challenge because it looked easy and I believed it would be good practice for concepts that I learned in my previous challenges. I was only partially right. This project was definitely still a challenge all on its own and humbled me quite a bit. The general development of the component was very similar to the previous projects, however the background images were a bit more complex than I had previously thought. This part of the project gave me the most trouble, and I spent a lot of time researching the best ways to deal with multiple background images and their positioning. I discovered some helpful forums and websites that I will definitely be using for future projects. Once again, Frontend Mentor has given me another fulfilling challenge that has put my frontend development skills to the test.

### Links

- Solution URL: [Solution on Frontend Mentor]()
- Live Site URL: [Live Site](https://ins140.github.io/Profile-Card-Component/)

## My process

As with all my projects, I start out with the HTML first. Next I develop classes for my elements and start to create my CSS file. I always start with the easy tasks like fonts and colors, positioning and margins/padding come afterwords. The last piece of the project was implementing the background images and their positioning depending on the viewport.

I did not use a live server this time and instead used npx serve from the terminal. Not as efficient since I had to refresh the page to see updates, but this project was small enough that it did not require live updates.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

During this challenge I learned a great deal about postioning and working with background images. I had a lot trouble trying to figure out how to correctly position the background images in the project, but with a some research and study I finally came to a conclusion.

```css
.bg-images {
    z-index: 0;
}

.img1 {
    position: fixed;
    left: -700px;
    top: -600px;
}
```
I learned how to create multiple classes for one element, shortening the amount of code I need for each styling effect.

```css
.flex-col {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
```
```html
<div class="card-container flex-col">
```

Lastly, I learned more ways to make my projects more accessible by hiding certain elements from screen-readers. This technique is especially useful for elements with no context or repeated phrases like company logos.

```html
<div aria-hidden="true" class="bg-images">
    <img class="img1" src="./assets/images/bg-pattern-top.svg" alt="background image">
    <img class="img2" src="./assets/images/bg-pattern-bottom.svg" alt="background image">
  </div>
```

### Continued development

Positioning and background images were a tough concept during this challenge, but going forward I feel like I will have a better understanding of it. Once again, I am also trying to implement accessibility as a huge part of my development process.

### Useful resources

- [W3Schools](https://www.w3schools.com) - The absolute best resource for anything CSS. It has been an absolutely invaluable resource during my studies.
- [CSS-TRICKS](https://css-tricks.com/positioning-offset-background-images/) - This article helped me understand the background image positioning

## Author

- Github - [INS140](https://github.com/INS140)
- Frontend Mentor - [@Ins140](https://www.frontendmentor.io/profile/INS140)