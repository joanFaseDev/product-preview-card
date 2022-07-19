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

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![](./images/screenshot_ProductPreviewCard.png)

### Links

- Solution URL: [Solution GitHub](https://github.com/joanFaseDev/FrontEnd-mentor-projects/tree/master/2.ProductPreviewCard)
- Live Site URL: [GitPage](https://joanfasedev.github.io/FrontEnd-mentor-projects/)

## My process

First and foremost, english isn't my first language so please forgive me for any mispellings or grammatical errors.

This challenge was about building a responsive product preview card. Being an aspiring front-end developper, i don't really have a method and my range of skills is quite limited but i figured i'll build the mobile version first because it seems easier to handle (there's less space to cover which means there's also less opportunities to screw up). I started out by creating some HTML elements i felt were needed (image, paragraph and button) then i added a couple of divs to act as containers because i pretty much decided by then that i will use flexbox to handle my card's layout. I didn't think much about it which was a big mistake (which i noticed as usual way later).

Once i deemed the HTML part satisfying, i worked on the Css part. I choose to use pixels for the width's container because i knew that a lot of things would be relative to this container and i felt that it will be way more easier to handle absolute units that relative ones. For all the others elements, i really tried to focus on rem mainly because even if it's a relative unit its value is almost always constant which appears very beginner friendly to me. I didn't set a height value because i read it was a bad habit and could potentially create overflow. Instead i created height where it was needed by using padding.

Overall the mobile design seemed like something i could manage. The only difficulty was the barred price and the cart icon. I tried to solve the first one by using the superscript tag but, even if the result was good, i felt the element wasn't made to be used like that so in the end i used _position: relative_ and some offset. I couldn't reproduce the blur effect though (i tried to play on opacity through the _text-decoration-color_ property but to no avail).

Then came the desktop design part which is the moment where i realized that the image used by the mobile version was different that the image used by the desktop one. Usually i would have fixed that with JavaScript but the challenge was limited to HTML/CSS so i tried to find useful ressources and ended up learning about and using the _picture_ and _source_ html elements which have very good synergy with media queries.

Finally i kept most of the css rules i wrote for the mobile design and changed my container in grid to assign each element to a specific area through rows and columns. Clearly it isn't perfect and there's probably a ton of ways to do this faster and better but the result seems pretty close to me and i thought i had spend enough time on that project and it was the moment to move on.

### Built with

- HTML5 (no semantic elements here)
- CSS + Grid

### What I learned

First and foremost, i realized the importance of planning at least in some ways before any actual coding. Had i done that here, i would have find out about the two different images needed and it would have saved me a lot of cold sweat.

I also learned about the _<picture>_ and _<source>_ HTML elements that i never used or heard about before. Still not sure i used them the right way but it felt pretty cool right then.

Finally i realized that the same design can be displayed in very unique way on two different screens. There was a moment during this project where i honestly believed i didn't used the right colors. Took me a little while to understand that it was just my desktop screen whose render where very different from my laptop one.

### Continued development

As i mentionned during the first project, i wish to train basic concepts of CSS. Things like positionning, length units, color systems, some layout global rules if there is. I see a lot of people using and talking about frameworks, preprocessor and things like that but i feel like i don't need them at the moment. Those are tools that seems really useful on bigger projects but that won't help at my level and worse, won't actually do anything to improve my knowledge of CSS.

## Author

- Website - [Jordan Falaise](https://joanfasedev.github.io/FrontEnd-mentor-projects/)
- Frontend Mentor - [@joanFaseDev](https://www.frontendmentor.io/profile/joanFaseDev)
