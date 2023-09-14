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
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![](./screenshot.jpg)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it. 

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

**Note: Delete this note and the paragraphs above when you add your screenshot. If you prefer not to add a screenshot, feel free to remove this entire section.**

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

### What I learned

First I learned that the svg file wasn't working! Need to ask about that in 
feedback. So I used Google icons instead--it worked pretty well and was easy.

Second I learned a lot of things that didn't work. I got a mobile version I was proud of, and a desktop version, but could not understand how to swap out the jpgs.

Finally stumbled across a Youtube video from Kevin Powell in which he does this challenge. The source attribute was new to me, but workrd like a charm. 

My version follows Kevin's pretty closely; one or two places he seemed to go a little overboard with the variables so I simplified. 


```html
<picture>
<!-- the missing piece of the puzzle. Thanks, Kevin!-->  
       <source
          srcset="images/image-product-desktop.jpg"
          media="(min-width: 600px)" />
       <img src="images/image-product-mobile.jpg" alt="product image" />   
</picture>          
```
```css
/* © Scott O'Hara, 2013 - 2023 */
 .visually-hidden:not(:focus):not(:active) {
  clip: rect(0 0 0 0); 
  clip-path: inset(50%);
  height: 1px;
  overflow: hidden;
  position: absolute;
  white-space: nowrap; 
  width: 1px;
}
```

### Continued development

Going to check out the various resources from the video on BEM naming conventions, visibility hidden, and <picture> and <source>, 'is' and 'where'.


### Useful resources

https://www.youtube.com/watch?v=B2WL6KkqhLQ&t=42s - this is the video of Kevin Powell's solution



*
