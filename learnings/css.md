# CSS Learning - Day 4

## What is CSS?

CSS (Cascading Style Sheets) is used to style HTML pages. HTML creates the structure of a webpage, while CSS controls its appearance, such as colors, fonts, spacing, layouts, and animations.

---

## Why CSS is Important

- Makes webpages visually attractive.
- Separates design from content.
- Improves user experience.
- Makes websites easier to maintain.
- Allows the same CSS file to style multiple pages.

---

## Ways to Add CSS

### 1. Inline CSS
CSS is written inside an HTML element using the `style` attribute.

Example:
```html
<h1 style="color: blue;">Hello</h1>
```

### 2. Internal CSS
CSS is written inside the `<style>` tag in the `<head>` section.

Example:
```html
<style>
    h1{
        color: blue;
    }
</style>
```

### 3. External CSS
CSS is written in a separate `.css` file and linked using the `<link>` tag.

Example:
```html
<link rel="stylesheet" href="style.css">
```

External CSS is the best method because it keeps HTML clean and allows one stylesheet to be used on multiple pages.

---

## CSS Selectors

Selectors are used to choose which HTML elements should be styled.

## CSS Selectors

### 1. Universal Selector (`*`)
Selects all elements on the webpage.

```css
*{
    margin: 0;
    padding: 0;
}
```

---

### 2. Element Selector
Selects all HTML elements of a specific type.

```css
p{
    color: blue;
}
```

---

### 3. Class Selector (`.`)
Selects all elements with the same class name.

```css
.card{
    background-color: white;
}
```

---

### 4. ID Selector (`#`)
Selects a single element with a unique ID.

```css
#header{
    color: navy;
}
```

---

### 5. Group Selector (`,`)
Applies the same style to multiple elements.

```css
h1, h2, p{
    font-family: Arial;
}
```

---
<br>

## File Path in CSS

A file path tells the browser where to find the CSS file or other resources like images. Writing the correct path is important so that the webpage can load the files successfully.

### Same Folder

If the HTML file and CSS file are in the same folder:

```html
<link rel="stylesheet" href="style.css">
```

---

### Using `./`

`./` represents the current folder.

```html
<link rel="stylesheet" href="./style.css">
```

---

### Going Back One Folder (`../`)

`../` moves one folder back.

Example:

```text
resume/
├── style.css
└── projects/
    └── profile-card/
        └── index.html
```

To access `style.css` from `profile-card/index.html`:

```html
<link rel="stylesheet" href="../../style.css">
```

## My Understanding

- I understood that HTML creates the structure of a webpage, while CSS makes it attractive.
- I learned that external CSS is the best way to style multiple webpages.
- I understood how different CSS selectors target specific HTML elements.
- I learned the importance of using correct file paths to link CSS files and images.
- I used Developer Tools to inspect HTML elements and test CSS styles.
- I built a styled resume, a profile card, a navigation bar, and a button collection to         practice these concepts.