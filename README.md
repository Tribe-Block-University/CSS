# Tribe Block - CSS Complete Guide

## Introduction
Cascading Style Sheets (CSS) is a stylesheet language used to control the presentation of HTML documents. It allows developers to separate content from design, making web pages more maintainable and visually appealing.

### What You Will Learn
- CSS Syntax & Selectors
- Box Model
- Flexbox & Grid
- Responsive Design
- Animations & Transitions
- CSS Variables & Custom Properties
- Best Practices & Performance Optimization

## 1. Getting Started with CSS
### What is CSS?
CSS (Cascading Style Sheets) describes how HTML elements should be displayed on the screen, paper, or other media.

### Adding CSS to HTML
There are three ways to apply CSS:
1. **Inline CSS:** Applied directly within an HTML tag using the `style` attribute.
2. **Internal CSS:** Defined within a `<style>` block inside the HTML `<head>`.
3. **External CSS:** Written in a separate `.css` file and linked using `<link>` in the `<head>`.

Example of external CSS:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Example</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Hello, World!</h1>
</body>
</html>
```

### Example CSS File (`styles.css`):
```css
body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    margin: 0;
    padding: 20px;
}

h1 {
    color: #333;
}
```

## 2. CSS Syntax & Selectors
CSS rules are written as:
```css
selector {
    property: value;
}
```
Example:
```css
p {
    color: blue;
}
```
### Common Selectors
- **Universal Selector (`*`)** - Selects all elements.
- **Element Selector (`p, h1, div`)** - Targets specific HTML tags.
- **Class Selector (`.classname`)** - Targets elements with a specific class.
- **ID Selector (`#idname`)** - Targets elements with a specific ID.
- **Attribute Selector (`[type="text"]`)** - Selects elements with specific attributes.

### Reference:
[MDN CSS Selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors)

## 3. CSS Box Model
The box model describes how HTML elements are structured in CSS.

### Components of the Box Model:
1. **Content** - The actual content inside an element.
2. **Padding** - Space between content and border.
3. **Border** - Surrounds the padding.
4. **Margin** - Space outside the border.

Example:
```css
div {
    width: 200px;
    padding: 10px;
    border: 5px solid black;
    margin: 20px;
}
```

### Reference:
[MDN Box Model](https://developer.mozilla.org/en-US/docs/Web/CSS/Box_model)

## 4. CSS Flexbox
Flexbox is a CSS layout model for arranging items efficiently.

### Example:
```css
.container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}
```
### Reference:
[MDN Flexbox](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox)

## 5. CSS Grid
CSS Grid is another powerful layout model for creating complex designs.

### Example:
```css
.container {
    display: grid;
    grid-template-columns: 1fr 2fr;
    gap: 10px;
}
```
### Reference:
[MDN Grid](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout)

## 6. Responsive Design
Responsive web design ensures websites work across different devices.

### Example:
```css
@media (max-width: 600px) {
    body {
        background-color: lightgray;
    }
}
```
### Reference:
[MDN Responsive Design](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Responsive_Design)

## 7. CSS Animations & Transitions
Enhance user experience with animations.

### Example:
```css
div {
    transition: background-color 0.5s ease-in-out;
}

div:hover {
    background-color: yellow;
}
```
### Reference:
[MDN Animations](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Animations)

## 8. CSS Variables
CSS Variables allow reusability and maintainability.

### Example:
```css
:root {
    --main-color: blue;
}

p {
    color: var(--main-color);
}
```
### Reference:
[MDN CSS Variables](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties)

## 9. Best Practices & Performance
- Use external CSS for maintainability.
- Minify CSS to improve performance.
- Avoid excessive use of `!important`.
- Optimize images and assets.

## Conclusion
CSS is essential for styling web pages and creating responsive, visually appealing designs. Keep practicing and exploring new CSS features to enhance your skills!

### Additional Resources
- [MDN Web Docs - CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [CSS Tricks](https://css-tricks.com/)
- [W3Schools - CSS](https://www.w3schools.com/css/)
