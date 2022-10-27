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
- [Author] Mr.Coder 
- [Acknowledgments] https://www.youtube.com/watch?v=9aDqk7jUMZQ

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements


## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Desktop-first workflow


**Note: These are just examples. Delete this note and replace the list above with your own choices**

### What I learned

I have used this opportunity to learn a different approach to creating a product card. I followed along the tutorial by Mr.Coder on Youtube. 

In the course of this tutorial I learned a few new things: 

1. How to remove a default padding from the browser 

```css

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

```

2. I have learned about the grid system. In this case, the grid system allows to create two columns. Use grid-template-column for two colums next to each otther. Also allow the max width for an image to be 100% so it does not overgrow the screen size and it would take the similar amount of height with the other column. 

```css
.grid {
    max-width: 700px;
    display: grid;
    grid-template-columns: 1fr 1fr;
    background-color: white;
    border-radius: 15px;
    /* To prevent image from overflowing the grid and causing the edges not to be rounded, use overflow property and make it hidden */
    overflow: hidden;
}

   .grid {
        /* make the grid column one fraction */
        grid-template-columns: 1fr;
    }

```

3.   Setting max-width prevents the image to be giant 

   ```css
    max-width: 100%;
    ```


4.  To make an image stick close to  the container make it inherit the display, so there is no unnecesary white spaces

```css
    display:inherit;
```

5.  Flex helps to spread the content items evenly.

```css
    display: flex;
    flex-direction: column;
    /* makes similar amount of space between the elements */
    justify-content: space-between;

```

5.   To makes the button take the whole line, make its width: 100%;

6. To prevent image from overflowing the grid and causing the edges not to be rounded, use overflow property and make it hidden 
   
   ```css
    overflow: hidden;

    ```

7. For images: 

```css
    /* make image smaller */
    .img img {
        max-height: 450px;
        /* to avoid white space on the side use width 100% */
        width: 100%;
        /* NEW THING: to avoid the image stretching set the object-fit. It will cut the extra part but not shrink it */
        object-fit: cover;
    }

    ``

### Useful resources

- [Mr.Coder on Youtube](https://www.youtube.com/watch?v=9aDqk7jUMZQ)  

## Author

- [Mr.Coder on Youtube](https://www.youtube.com/watch?v=9aDqk7jUMZQ)


