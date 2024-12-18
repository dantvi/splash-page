# Splash Page

The Splash Page project is a visually captivating landing page designed to showcase branding and provide users with easy access to download mobile apps. Built with HTML, CSS, and JavaScript, it features a responsive layout and dynamic background toggling functionality.

This project was developed as part of the course "JavaScript Web Projects: 20 Projects to Build Your Portfolio" by Zero To Mastery.

## Table of contents

- [Splash Page](#splash-page)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
    - [Screenshot](#screenshot)
    - [Links](#links)
    - [Built with](#built-with)
    - [What I learned](#what-i-learned)
    - [Useful resources](#useful-resources)
  - [Author](#author)
  - [Acknowledgments](#acknowledgments)

## Overview

The Splash Page project combines modern design and functionality to create a seamless user experience. Users can:
- View branding and promotional content for a mobile app.
- Dynamically switch between different background styles for enhanced interactivity.
- Enjoy a fully responsive layout optimized for various devices.

### Screenshot

![](./screenshot.png)

### Links

- Live Site URL: [DT Code](https://splash-page.dtcode.se/)

### Built with

- HTML5: Semantic structure to ensure accessibility and usability.
- CSS3:
  - Gradients and linear backgrounds for visual appeal.
  - Flexbox for layout structure.
  - Responsive design techniques for various screen sizes.
- JavaScript (ES6+):
  - Event handling to implement background toggling.
  - Dynamic class manipulation for seamless background transitions.

### What I learned

This project allowed me to refine my skills in:
- CSS Gradients: Creating visually appealing backgrounds with linear and radial gradients.
- Dynamic Class Manipulation: Using JavaScript to toggle classes for interactive design elements.
- Responsive Design: Developing layouts that adapt to different screen sizes.
- Landing Page Best Practices: Structuring content and calls-to-action for effective user engagement.

The following example demonstrates how the dynamic background toggling is implemented:

```js
function changeBackground(number) {
    let previousBackground;
    if (body.className) {
        previousBackground = body.className;
    }
    body.className = '';
    switch (number) {
        case '1': 
            return (previousBackground === 'background-1' ? false : body.classList.add('background-1'));
        case '2':
            return (previousBackground === 'background-2' ? false : body.classList.add('background-2'));
        case '3':
            return (previousBackground === 'background-3' ? false : body.classList.add('background-3'));
        default:
            break;
    }
}
```

### Useful resources

- [MDN Web Docs: CSS Gradients](https://developer.mozilla.org/en-US/docs/Web/CSS/gradient) - A comprehensive guide to creating linear and radial gradients.
- [MDN Web Docs: Event Listeners](https://developer.mozilla.org/en-US/docs/Web/API/EventTarget/addEventListener) - Helped implement the background toggling functionality.

## Author

- GitHub - [@dantvi](https://github.com/dantvi)
- LinkedIn - [@danieltving](https://www.linkedin.com/in/danieltving/)

## Acknowledgments

Special thanks to Zero To Mastery for their inspiring course and to MDN Web Docs for their detailed documentation, which made implementing this project seamless and enjoyable.
