# Frontend Mentor - News homepage solution

This is a solution to the [News homepage challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/news-homepage-H6SWTa1MFl). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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


## Overview

### The challenge

Users should be able to:

- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Screenshot

![](https://github.com/carolmedici/news-homepage/blob/main/images/print/desktop.png)
![](https://github.com/carolmedici/news-homepage/blob/main/images/print/menu-mobile.png)
![](https://github.com/carolmedici/news-homepage/blob/main/images/print/mobile-at.png)


### Links

- Solution URL: [https://github.com/carolmedici/news-homepage](https://github.com/carolmedici/news-homepage)
- Live Site URL: [https://carolmedici.github.io/news-homepage/](https://carolmedici.github.io/news-homepage/)

## My process

### Built with

- Semantic HTML5
- CSS custom properties
- Responsive media query
- CSS Grid
- Mobile-first workflow
- Javascript


### What I learned

I learned how to make hamburger menu in JS and practiced HTML and CSS skills.

Check out some of my code below:

```html
<nav>
    <div class="logo"><img src="images/logo.png" alt="Website logo"></div>
   <div id="menu">
       <div id="menu-bar" onclick="menuOnClick()">
        <div id="bar1" class="bar"></div>
        <div id="bar2" class="bar"></div>
        <div id="bar3" class="bar"></div>
      </div>
      <nav class="nav" id="nav">
        <ul>
            <li><a  href="#">Home</a></li>
            <li><a  href="#">New</a></li>
            <li><a  href="#">Popular</a></li>
            <li><a  href="#">Trending</a></li>
            <li><a  href="#">Categories</a></li>
       </ul>
       
   </div>
</nav>
<div class="menu-bg" id="menu-bg"></div>
```
```css
nav{
        display: flex;
        justify-content: space-between;
        margin: 4rem;
        margin-bottom: 4rem;
        margin-top: 5rem;
    }


    #menu {
        z-index: 2;
        background-color: white;
    }
      
    #menu-bar {
        width: 4.5rem;
        height: 4rem;
        margin: 6rem 4rem 0 2rem;
        cursor: pointer;
    }
      
    .bar {
        height: 5px;
        width: 100%;
        background-color: var(--accent-color);
        display: block;
        border-radius: 5px;
        transition: 0.3s ease;
```
```js
function menuOnClick() {
    document.getElementById("menu-bar").classList.toggle("change");
    document.getElementById("nav").classList.toggle("change");
    document.getElementById("menu-bg").classList.toggle("change-bg");
    
   
  }
```


### Continued development

I will keep learning and practicing my JS skills



### Useful resources

- [How TO - Mobile Navigation Menu](https://www.w3schools.com/howto/howto_js_mobile_navbar.asp) - This site taught me how to make a hamburger menu.


## Author

- LinkedIn - [Carolina Médici](https://www.linkedin.com/in/carolina-medici/)
- Frontend Mentor - [@carolmedici](https://www.frontendmentor.io/profile/carolmedici)
