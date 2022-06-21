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
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <link rel="stylesheet" href="/style.css" />
    <link
      rel="shortcut icon"
      type="image/x-icon"
      href="https://cdn.glitch.global/c317d3b3-bbb5-4289-a549-1f8262efa030/favicon-32x32.png?v=1655448374803"
    />
  </head>
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
</html>

```

```css
@import url("https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600&display=swap");

body {
  min-height: 100vh;
  min-width: 100vw;
  background: #0d192c;
  display: flex;
  align-items: center;
  justify-content: center;
}
.eye {
  position: absolute;
  width: 302px;
  height: 302px;
  border-radius: 8px;
  background: #00fff8;
  mix-blend-mode: normal;
  opacity: 0.5;
  border-radius: 8px;
  display: none;
}

#card {
  position: relative;
  background: #15263f;
  width: 350px;
  height: 596px;
  border-radius: 15px;
}

.hover-image {
  position: absolute;
  width: 44px;
  display: none;
}

#flex-container {
  display: flex;
  position: relative;
  padding: 24px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.main-image {
  display: flex;
  position: relative;
  width: 302px;
  height: 302px;
  border-radius: 8px;
}
#flex-container:hover .eye {
  display: block;
  cursor: pointer;
}
#flex-container:hover .hover-image {
  display: block;
  cursor: pointer;
}

h1 {
  font-family: "Outfit", sans-serif;
  font-style: normal;
  font-size: 22px;
  font-weight: 600;
  cursor: pointer;
  color: #00fff8;
  margin-top: 0px;
  margin-bottom: 0px;
}
.main-text {
  width: 302px;
  height: 28px;
  display: flex;
  margin-left: 24px;
}
.description-box {
  width: 302px;
  height: 52px;
  display: flex;
  margin: 24px;
}
.description {
  font-family: "Outfit", sans-serif;
  font-style: normal;
  font-size: 18px;
  font-weight: 300;
  color: #8bacd9;
  margin-top: 0px;
  margin-bottom: 0px;
}
.eth {
  width: 93.48px;
  height: 20px;
  display: flex;
  align-items: center;
  margin-top: 0px;
  margin-left: 24px;
  justify-content: center;
}
.eth-text {
  width: 75px;
  height: 20px;
  margin: 0 auto;
  font-family: "Outfit", sans-serif;
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 20px;
  color: #00fff8;
}
.time {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 95.36px;
  height: 20px;
  margin-right: 26px;
  margin-top: 0px;
}

.wrapper {
  margin-top: 0px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.time-text {
  margin: 0 auto;
  font-family: "Outfit", sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 20px;
  color: #8bacd9;
}
hr {
  display: flex;
  margin-top: 24px;
  width: 302px;
  background: #2e405a;
  height: 1px;
  border-style: none;
}
.avatar {
  width: 33px;
  border: 1px solid #ffffff;
  border-radius: 50px;
}
.bottom-wrapper {
  margin-left: 24px;
  display: flex;
  justify-content: ;
  align-items: center;
}
.creator {
  margin-left: 16px;
  color: #8bacd9;
  font-family: "Outfit", sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 20px;
}
#color-stack {
  color: #00fff8;
  text-decoration: none;
}

```

## Author

- Website - [Giorgi Mekantsishvili](https://www.your-site.com)
- Glitch - [Gmekantsis](https://glitch.com/@gmekantsis)
