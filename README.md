# Frontend Mentor - NFT preview card component

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](https://cdn.glitch.global/c317d3b3-bbb5-4289-a549-1f8262efa030/overview.png?v=1655798091110)
  - [The challenge](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj)
  - [Screenshot](https://cdn.glitch.global/c317d3b3-bbb5-4289-a549-1f8262efa030/NFT%20card.png?v=1655798179878)
  - [Built with](https://www.lambdatest.com/blog/wp-content/uploads/2018/11/JPG-2.jpg)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Challenge was to create pixel-perfect copy of the project from scratch.

### Screenshot

![](https://cdn.glitch.global/c317d3b3-bbb5-4289-a549-1f8262efa030/NFT%20card.png?v=1655798179878)

### Links

- Solution URL: [Add solution URL here](https://glitch.com/edit/#!/nft-card-review-)
- Live Site URL: [Add live site URL here](https://nft-card-review-.glitch.me)

## My process

First, I assembled all the necessary components in the HTML and then I styled it with using CSS.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid

### What I learned

```html
<body>
    <div id="card">
      <div id="flex-container">
        <img
          class="main-image"
          src="https://cdn.glitch.global/c317d3b3-bbb5-4289-a549-1f8262efa030/image-equilibrium.jpg?v=1655448318028"
        />
        <span class="eye"></span>
        <img
          class="hover-image"
          src="https://cdn.glitch.global/c317d3b3-bbb5-4289-a549-1f8262efa030/icon-view.svg?v=1655448345208"
        />
      </div>
      <span class="main-text"><h1>Equilibrium #3429</h1></span>
      <span class="description-box"
        ><p class="description">
          Our Equilibrium collection promotes balance and calm.
        </p></span
      >
      <div class="wrapper">
        <div class="eth">
          <img
            class="eth-image"
            src="https://cdn.glitch.global/c317d3b3-bbb5-4289-a549-1f8262efa030/icon-ethereum.svg?v=1655448354629"
          />
          <p class="eth-text">0,041 ETH</p>
        </div>
        <div class="time">
          <img
            class="clock-image"
            src="https://cdn.glitch.global/c317d3b3-bbb5-4289-a549-1f8262efa030/icon-clock.svg?v=1655448366509"
          />
          <p class="time-text">3 days left</p>
        </div>
      </div>
      <hr />
      <div class="bottom-wrapper">
        <img
          class="avatar"
          src="https://cdn.glitch.global/c317d3b3-bbb5-4289-a549-1f8262efa030/image-avatar.png?v=1655448333550"
        />
        <p class="creator">
          Creation of <a id="color-stack" href="#">Jules Wyvern</a>
        </p>
      </div>
    </div>
  </body>
```

```css
#flex-container:hover .eye {
  display: block;
  cursor: pointer;
}
#flex-container:hover .hover-image {
  display: block;
  cursor: pointer;
}
```

## Author

- Website - [Giorgi Mekantsishvili](https://www.your-site.com)
- Glitch - [Gmekantsis](https://glitch.com/@gmekantsis)
