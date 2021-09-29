# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [What I struggled with](#what-i-struggled-with)
  - [Useful resources](#useful-resources)
- [Author](#author)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![](./desktop-view.jpg)
![](./mobile-view.jpg)


### Links

- Solution URL: [https://github.com/graficdoctor/stats-preview-card-component](https://github.com/graficdoctor/stats-preview-card-component)
- Live Site URL: [https://stats-preview-card-component-five-pi.vercel.app/](https://stats-preview-card-component-five-pi.vercel.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

It was quite a challenge to figure out how to do the color overlay on the image. I ran into cascading-issues when I applied one, but the other didn't work on mobile view and been going back and forth to some solutions until I found the `mix-blend-overlay` and set it to `multiply` on `img`. 
I found this solution in one of the solutions on Front End Mentor, though I don't remember which one.

```
img {
  width: 100%;
  display: block;
  object-fit: cover;
  mix-blend-mode: multiply;
}
```

I somehow also ended up struggling to use `space-between` on `.preview-card-numbers`. For this I used Firefoxs' Inspector and toyed with the settings while visualising the flexbox. After setting a width of 100% to this element, it just worked.

```
.preview-card-numbers {
  width: 100%;
  flex-direction: row;
  justify-content: space-between;
}
```

### What I struggled with

I usually find it very easy to center my div, but as you'll see on mobile view, I didn't manage this time. I couldn't find a solution for this.

### Useful resources

- [CSS Tricks](https://css-tricks.com/almanac/properties/m/mix-blend-mode/) - It's only after applying the mix-blend-overlay I looked it up on CSS Tricks.


## Author

- Website - [Katrien S.](https://www.katriens.be)
- Frontend Mentor - [@graficdoctor](https://www.frontendmentor.io/profile/graficdoctor)
- Twitter - [@graficdoctor](https://www.twitter.com/graficdoctor)
