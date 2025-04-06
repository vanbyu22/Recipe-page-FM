# Frontend Mentor - Recipe Page Challenge Solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)

## Overview

### Screenshot

![Final Result](https://github.com/vanbyu22/Recipe-page-FM/blob/2768cb3e9c9ab3a2870e48a8c830a81763a2c5c6/Recipe-page-main-fullsize.png)

### Links

- Challenge URL on Frontend Mentor: (https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm)

## My process

A little more challenging than the previous projects but I actually enjoyed this one. Comprised of sections and divs within a main container.

### Built with

- Semantic HTML5 & CSS on VS Code (with Prettier extension)

### What I learned

I've learned indentation or spacing between the bullet points and texts by adding left padding to the < li > as shown below:

```CSS
.ingredients li,
.prep-box li,
.instructions li {
  padding-left: 25px; /*gives space between bullet points and text*/
}
```

But when I got to the last section "Nutrition", I was having trouble figuring out how to format the data like keeping all the texts lined up without using < tables >. So I ended up asking AI (MS Copilot to be exact) to suggest how to go about it. After giving me some markup and CSS (with plenty of errors), I tweaked it with my original markup and figured out by giving the spans 100% width, the data is able to maintain its responsive formatting even when screen sizes change.

```HTML
<div class="nutrition-item">
  <span class="nutrition-label">Calories</span>
  <span class="nutrition-value">277 kcal</span>
</div>
```

```CSS
.nutrition-label {
  padding-left: 25px; /*indentation again*/
  width: 100%;
}

.nutrition-value {
  width: 100%;
  font-weight: bold;
  text-align: left;
  color: hsl(14, 45%, 36%);
}
```

Finally, I've incorporated media queries for the mobile version. I've got a better understanding of it from Colt Steele's Web Developer Bootcamp 2025 from Udemy.

### Useful resources

- [Stack Overflow - CSS: Control space between bullet and < li > ](https://stackoverflow.com/questions/4373046/css-control-space-between-bullet-and-li)

- [The Web Developer Bootcamp 2025 by Colt Steele via Udemy](https://www.udemy.com/course/the-web-developer-bootcamp/?couponCode=KEEPLEARNING)
