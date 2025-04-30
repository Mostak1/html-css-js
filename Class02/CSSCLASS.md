# **CSS Learning Notes with Code Examples**

## **1. Introduction to CSS**
CSS (Cascading Style Sheets) is used to style HTML elements. It controls layout, colors, fonts, and more.

### **Basic Syntax**
```css
selector {
  property: value;
}
```
Example:
```css
p {
  color: blue;
  font-size: 16px;
}
```

---

## **2. Ways to Add CSS**
### **Inline CSS (Inside HTML Tag)**
```html
<p style="color: red; font-size: 20px;">This is a paragraph.</p>
```

### **Internal CSS (Inside `<style>` Tag)**
```html
<head>
  <style>
    p {
      color: green;
    }
  </style>
</head>
```

### **External CSS (Separate `.css` File)**
```html
<head>
  <link rel="stylesheet" href="styles.css">
</head>
```
In `styles.css`:
```css
p {
  color: purple;
}
```

---

## **3. CSS Selectors**
### **Element Selector**
```css
h1 {
  text-align: center;
}
```

### **Class Selector (`.`)**
```css
.highlight {
  background-color: yellow;
}
```
```html
<p class="highlight">This is highlighted.</p>
```

### **ID Selector (`#`)**
```css
#header {
  font-size: 24px;
}
```
```html
<h1 id="header">Welcome!</h1>
```

### **Grouping Selectors**
```css
h1, h2, h3 {
  font-family: Arial;
}
```

### **Descendant Selector**
```css
div p {
  color: blue;
}
```
(Selects all `<p>` inside `<div>`)

---

## **4. Box Model**
Every element is a box with:
- **Content** – The actual text/image.
- **Padding** – Space inside the border.
- **Border** – Edge around padding.
- **Margin** – Space outside the border.

```css
.box {
  width: 200px;
  padding: 20px;
  border: 2px solid black;
  margin: 10px;
}
```

---

## **5. Display Properties**
### **Block (Takes Full Width)**
```css
div {
  display: block;
}
```

### **Inline (Takes Only Needed Width)**
```css
span {
  display: inline;
}
```

### **Inline-Block (Inline but Adjustable)**
```css
button {
  display: inline-block;
  width: 100px;
}
```

### **Flexbox (Modern Layout)**
```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

### **Grid (2D Layout)**
```css
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto;
  gap: 10px;
}
```

---

## **6. Positioning**
### **Static (Default)**
```css
div {
  position: static;
}
```

### **Relative (Adjustable from Normal Position)**
```css
div {
  position: relative;
  top: 10px;
  left: 20px;
}
```

### **Absolute (Relative to Parent)**
```css
div {
  position: absolute;
  top: 50px;
  left: 50px;
}
```

### **Fixed (Stays in Place on Scroll)**
```css
.navbar {
  position: fixed;
  top: 0;
}
```

### **Sticky (Switches Between Relative & Fixed)**
```css
.header {
  position: sticky;
  top: 0;
}
```

---

## **7. Colors & Backgrounds**
### **Text Color**
```css
h1 {
  color: #FF5733; /* Hex */
  color: rgb(255, 87, 51); /* RGB */
  color: hsl(12, 100%, 60%); /* HSL */
}
```

### **Background Color**
```css
body {
  background-color: lightblue;
}
```

### **Background Image**
```css
div {
  background-image: url("image.jpg");
  background-size: cover;
}
```

---

## **8. Pseudo-classes & Pseudo-elements**
### **Pseudo-classes (`:`)**
```css
a:hover {
  color: red;
}

button:active {
  background: black;
}

li:nth-child(odd) {
  background: #f2f2f2;
}
```

### **Pseudo-elements (`::`)**
```css
p::first-letter {
  font-size: 2em;
}

p::after {
  content: " - Read more";
}
```

---

## **9. Transitions & Animations**
### **Transition (Smooth Hover Effect)**
```css
button {
  transition: background 0.5s ease;
}

button:hover {
  background: blue;
}
```

### **Keyframe Animation**
```css
@keyframes slide {
  from { transform: translateX(0); }
  to { transform: translateX(100px); }
}

.box {
  animation: slide 2s infinite;
}
```

---

## **10. Responsive Design (Media Queries)**
```css
@media (max-width: 600px) {
  body {
    background: lightgreen;
  }
}
```

---

### **Summary**
- CSS styles HTML elements.
- Use selectors (`element`, `.class`, `#id`).
- Box model: `margin`, `border`, `padding`, `content`.
- Layout: `flexbox`, `grid`, `position`.
- Effects: `hover`, `transition`, `animation`.
- Responsive: `@media`.

**Practice these concepts to master CSS! 🚀**