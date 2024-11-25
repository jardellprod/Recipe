# Frontend Mentor - Recipe page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

## Overview

### Screenshot

#### Desktop

![](/images/screenshot_final_output_desktop.png)

#### Mobile

![](/images/iphone_screenshot.png)

### Links

- Solution URL: [Recipe](https://github.com/jardellprod/Recipe)
- Live Site URL: [https://jardellprod.github.io/Recipe/](https://jardellprod.github.io/Recipe/)

## My process

### Built with

- HMTL5
- CSS
- Flexbox
- CSS Grid

### What I learned

In the original design shared, there was a gap at the top and at the bottom of the recipe container, also it looked as thought the recipe was centered in the middle of the page. I wanted to do something similar, but ran into an issue when using flex or grid. Essentially
I ran into an issue with adding a gap at the top and bottom of the page. when I center the content using flex or grid it will automatically add a gap at the top and bottom if there is space. However b/c the content is long I had to make sure based on a certain height add a gap automatically, and still allow the content to take more space than what is made available by the parent.

I also had an issue with adding space between the marker and content in the li element. I essentially had to hide the marker, use another notation to get the bullet points or numbers as an additional item in the flex li container. This gave me more styling flexibility.

Honestly i don't know what my life would be like without Grid or flex.

```css
body {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  background-color: hsl(30, 54%, 90%);
}
```

Also I didn't know how to make a horizontal table, where the headers are on the first column of the table, so I learned to do that using hte th element.

```html
<table>
  <tbody>
    <tr>
      <th scope="row">Calories</th>
      <td>277kcal</td>
    </tr>
    <tr>
      <th scope="row">Carbs</th>
      <td>0g</td>
    </tr>
    <tr>
      <th scope="row">Protein</th>
      <td>20g</td>
    </tr>
    <tr>
      <th scope="row">Fat</th>
      <td>22g</td>
    </tr>
  </tbody>
</table>
```

I also learned to use the clamp function for text. It has some cons, but overtime I think I will get better at using it.

Finally I learned to use Media queries, which helped make the site more mobile friendly.

### Continued development

I am proud that I pushed through, there were some difficult styling challenges, and I'm sure I could have had cleaner code. I hope to improve on this as I practice more, and again I really need to use css variables. I think next time I'll define them first, color, and font-weight or any sort of clamp style will be defined at the top.

## Author

- Frontend Mentor - [@jardellprod](https://www.frontendmentor.io/profile/jardellprod)
