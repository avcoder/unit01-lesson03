---
# You can also start simply with 'default'
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: /assets/intro.jpg
# some information about your slides (markdown enabled)
title: Software Development | Foundations
info: |
  ## Software Development | Foundations
# apply unocss classes to the current slide
class: text-left
drawings:
  persist: false
transition: slide-left
mdc: true
---

# CSS - part 1/3
Software Development Bootcamp - Circuit Stream
- [ ] Describe how CSS is used to style website
- [ ] Modify an HTML document using CSS
- [ ] Use `div` element and class attribute to change the layout of a website

<div class="abs-br m-6 text-xl">
  <a href="https://github.com/slidevjs/slidev" target="_blank" class="slidev-icon-btn">
    <carbon:logo-github />
  </a>
</div>

<!--
TODO: fill in anchor href above to point to github repo for these slides
- take attendance
- verify previous zoom video uploaded
-->

---
transition: slide-left
---

# Q&A
(5 min)

- 🪲 Included question and answers on "Lesson 2 + FAQ" in LMS
- 📝 More clarification on assignments (i.e. due dates, when to start, by topics)


<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<!--
Q: assignments clarification
A: 
- I put due dates in Content Class Recordings
- "Personal Website" is same thing as "Portfolio" assignment
- divided by topic
- official start date is when we finish lesson 1 of that topic; as gradual knowledge is built, can continue to work on assignment

-->

---
transition: slide-left
---

# Summary from Last Class
(10 min)

- 🏃‍♀️‍➡️ Recap on how HTML5 works
   - What's the very first, top-most HTML tag?
   - What attribute does `<html>` tag contain that had a value of "en"?
   - What goes inside the `<head>` tag?
   - How can I change the text on my browser tab? 
   - What tag encapsulates the visible portion of the webpage?
   - What's the acronym that describes what you see when you Inspect a webpage?
- 🏷️ Most common tags:
   - `<h1>` to `<h6>`, `<p>`, `<span>`, `<a>` `<img>` `<ul> <li>` `<input>` `<button>` `<!-- comment -->`

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<!--
- Inspecting DOM trains your eye to focus on what tags you're looking for amongst the DOM noise
- React DevTools similar
- Will use this every day in your professional life
- My last slide from previous class had a link to layout elements
- Note: Inspect > Elements > What was injected if using Live Server?
-->

---
layout: image-right
transition: slide-left
image: /assets/patio01.png
backgroundSize: 400px 250px
class: text-left
---

# Exercise: How to create a stylesheet
(5 min) Use my [Menu Exercise](https://github.com/avcoder/css-temp2) from Last Class
|                                                     |                             |
| --------------------------------------------------- | --------------------------- |
| 📝 1. Create File 
| 🔗 2. Link CSS File within `<head>` via 
`<link rel="stylesheet" href="style.css">`
| 📏 3. Add CSS Rules


<!-- 
- https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Styling_basics/Getting_started
1. File extension must end with `.css` (ex: style.css)
2. Link
3. Define sets of properties/values for each target 

- Note: CSS origins comes from print design
- Artsy types (ex: Photoshop) will love CSS
-->

---
transition: slide-left
---

# Exercise: CSS & HTML
(5 min) How CSS and HTML work together

- 🖼️ Most common HTML [Layout Elements](https://www.w3schools.com/html/html_layout.asp)
- `<header>` `<nav>` `<section>` `<article>` `<div>` `<footer>`   
- Move Plates, Drinks, Desserts to containers
- https://www.w3schools.com/html/html_layout.asp

<!-- 
- put your menu sections inside the containers tags
-->

---
transition: slide-left
---

# Anatomy of a stylesheet
(5 min)
|                                                     |                             |
| --------------------------------------------------- | --------------------------- |
| 🎯 CSS Selectors | Identify the HTML element(s) you want to style |
| ⚙️ CSS Properties | Define aspect of an element's appearance `background-color` |
| 🔢 CSS Values      | Define value associated with property  `green` |
| 🥂 CSS Declarations | Contains property and value pair `background-color: green;`    |
| 💬 CSS Comments | `/* This is a comment in CSS */` |

```css
/* CSS Rule */
#plates {
   background-color: yellow;
   color: brown;
}
```

<!-- 
-->

---
transition: slide-left
---

# Inline & Internal CSS
(5 min) 
- Good to be aware of these options
- But inline and internal styles is considered bad practice (hard to maintain)


## Inline CSS

`<h1 style="background-color: green; color: brown">Plates</h1>`

## Internal CSS

```html
<style>
   #plates {
      background-color: green;
      color: brown;
   }
</style>
```

<!-- 
- Maintain: One of the hardest problems you'll discover in professional coding is maintaining code
- How easy can you make a change in your code without breaking something else?
-->

---
transition: slide-left
---

# Selectors, declarations & Syntax
(15 min) How to create styles

```css
.card {
    display: flex;
    justify-content: space-between;
    width: 90%;
    margin: 0 auto;
    background-color: #f8f8f8;
}

.btn {
    background-color: #262626;
    color: #ffffff;
    padding: 16px 24px;
    margin-top: 25px;
    display: inline-block;
    text-decoration: none;
    width: 210px;
    text-align: center;
}
```

<!--
- Note the colon to separate property vs value
- Note the semicolon to end a declaration
-->

---
layout: image-right
transition: slide-left
image: /assets/chriscoyier.png
backgroundSize: 500px 400px
class: text-left
---

# 10 minute break
<br/>

🍦 Cool Tips, Trends and Resources:
- 📦 [Box Model](https://css-tricks.com/the-css-box-model/)
- 🍽️ [CSS Diner](https://flukeout.github.io/)
- 🐸 [Flexbox Froggy](https://flexboxfroggy.com/)
- 🔠 [MixFont Pairing](https://www.mixfont.com/Yellowtail+Radley)
- 🪄 [CSS Almanac](https://css-tricks.com/almanac/)
- 👽 [Why is CSS So Weird?](https://www.youtube.com/watch?v=aHUtMbJw8iA)

---
transition: slide-left
---

# Exercise: Styling a website
(45 min) Follow along using the menu website from last class

1. Add and apply Google Font for paragraph, and h2
2. Set Font sizes for `<h2>` `<h3>` `<li>` `<p>`
3. Box Model, create `<div>` box and play with `padding, border, margin`
4. Play with `width, background-color, color, text-shadow, display`
5. Style the `<body>`, rest of `.card` including `<button>`
6. Style the `<section>`, `<article>` `<aside>`
7. Create and style `<main>` and embed a google map
8. Style `<header> <footer>`

<!-- 
- Follow:
https://developer.mozilla.org/en-US/docs/Learn_web_development/Getting_started/Your_first_website/Styling_the_content
- Cascading
- use
-->

---
transition: slide-left
---

# 5 minute break
<br/>

🍦 Cool Tips, Trends and Resources:
- 🌪️ [Thinking Like a FrontEnd Dev](https://www.youtube.com/watch?v=tI0MGJe_ojU)
- 💪 [CSS Flexbox Layout Guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- 🦸‍♀️ [Hero Patterns](https://heropatterns.com/)
- 🖼️ [Perfect Full Page Background Image](https://css-tricks.com/perfect-full-page-background-image/)
- ☑︎ [State of CSS Survey](https://2024.stateofcss.com/en-US/usage/#what_do_you_use_css_for)

---
transition: slide-left
---

# Exercise Using CSS to create a layout
(40 min) Group exercise

-  Use the menu that you created last class and change it according to your liking
- Tip: Use `<div>` elements then add classes to create specific styles for specific elements

---
transition: slide-left
---

## For homework:

- Take the musician website you created from previous lesson, and change the way it looks using CSS

- Apply what you've learned so far to your "Personal Website" assignment (aka Portfolio assignment)

<!--
- take attendance
-->
