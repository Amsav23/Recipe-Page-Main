# Frontend Mentor - Recipe page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Examples of Code I'm Proud of](#examples-of-code-that-i-am-proud-of)
  - [Notes to Remember](#notes-to-remember)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)


## Overview

### Links

- Solution URL: [https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm]
- Live Site URL: [https://recipe-page-savarese.netlify.app/]

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Desktop-first workflow
- Flexbox
- [GitHub](https://github.com/) - Version control and collaboration



### What I learned

While working through this project, I wanted to slow down and really take my time reading through the README files provided, and follow along with the provided style-guide to accurately style this landing page. Up until this project, in all my previous projects, I never really tried to slow down and read through all the directions I was given, nor carefully read what the Figma file was aiming for.

Instead, I would typically bulldoze head first into a project and rush to make it styled just like how it was in its Figma file. This approach of diving in head first with no direction *clearly* wasn't working, because I wasn't understanding ***why*** I was doing what I was doing. I didn't think to **plan out** what the page needed to say, and now I realized that if I *don't* plan the layout, how in the world would I be able to style it **properly**?

I realized that it's very important for me to make sure I **understand** what the project is asking of me, and by carefully working through each step and each line of code, I will become faster, more efficient at coding, and I will retain the process better.

Sometimes I did ask ChatGPT for help when I struggled on certain sections of styling. Sometimes I didn't know how to style things **separately**, like coloring bulleted lists and numbered lists separately from their text. I also asked ChatGPT about how to create lines underneath text, like in the Nutrition section where there are long lines under each category like Calories, Carbs, etc. That is actually a design struggle I had previously encountered in an earlier project I had done. So it was nice to finally see how to style the lines properly!

It was also important for me to recognize how different sections of **HTML** sometimes needs to be **in their own containers**, because that definetely affects **how it will be styled** in CSS. Using **borders** and **background colors** on containers has helped me **visualize** where HTML sections are on the page, how much room they take up, and where I can move them around using Flexbox.


### Examples of code that I am proud of:

```html
<ul>
  <li><strong>Total:</strong> Approximately 10 minutes</li>
  <li><strong>Preparation:</strong> 5 minutes</li>
  <li><strong>Cooking:</strong> 5 minutes</li>
</ul>
```
```css
/* Set the color for the bullet points and numbers */
.ingredients-container ul li::marker, ol li::marker {
    color: var(--Nutmeg);
    font-weight: 700;
}

/* Using a root selector for CSS */
* {
    --Nutmeg: hsl(14, 45%, 36%);
    --DarkRaspberry: hsl(332, 51%, 32%);
    --blue: hsl(228, 45%, 44%);
}

/* Standardizing the size of the page */
body {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

/* Combining HTML classes for styling */
p, h3, li, .nutrition-item {
    font-family: var(---pgFonts);
}
```


### Notes to Remember:

It's important to create a **root selector** for **variables** that I want to use, and may need to change in the future. It makes changing styling easier, and it **avoids** writing extra, **unnecessary code** over and over again.

Make sure you start by zero-ing out the **default style** of the page you're working on. It's important for **consistency** in the appearance of elements across different browsers and devices, **predictability** for the layout and appearance of elements, and **easier debugging** when you start with a clean slate. This creates a **manageable starting point** for **styling**.

**ul li::marker, ol li::marker:** **Targets only the markers** (bullets or numbers) in the list items. This approach ensures that only the **bullet points** and **numbered list** markers change color, while the text remains unaffected.

*Checking out [The Markdown Guide](https://www.markdownguide.org/) to learn more on how to write markdown.*


### Continued development

**In the future, I'd like to focus on:** making sure I **understand** what the project is asking me to do; **Create a plan** of what to work on first, and *then* move on to the next section of the project; Gain a better understanding of **CSS properties** and how they **affect each other** on the page; And look into **specific CSS properties**, like when styles use double colons "::" like this (**ol li::marker**), and **why** that is used; I'd like to work on understanding how **Media Queries** work, what general sizing to use, when to use it, and what elements to change with it.


### Useful resources

- [ChatGPT](https://chatgpt.com/) - This helped me when I was unsure of how to style specific elements in CSS. It also just helped me in general when I was confused on a concept, I'd ask ChatGPT for a deeper explanation of **why** things were the way they were.


## Author

- Website - [Amyln Savarese]
- Frontend Mentor - [@Amsav23](https://www.frontendmentor.io/profile/Amsav23)
