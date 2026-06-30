# Day 5 - CSS Fundamentals (Part 2)

## 1. Naming Conventions

Writing meaningful and consistent names makes CSS easier to understand and maintain.

### Good Examples
```css
.navbar {}
.main-container {}
.login-form {}
.profile-card {}
```

### Bad Examples
```css
.box1 {}
.test {}
.xyz {}
```

**Best Practice**
- Use lowercase letters.
- Separate multiple words with hyphens (`-`).
- Use meaningful names based on the purpose.

---

## 2. Embed Code (Internal CSS)

Internal CSS is written inside the `<style>` tag within the `<head>` section.

```html
<head>
    <style>
        h1{
            color: blue;
        }
    </style>
</head>
```

Use it when styling a single webpage.

---

## 3. Font Style

The `font-style` property changes the appearance of text.

```css
p{
    font-style: italic;
}
```

Values:
- `normal`
- `italic`
- `oblique`

---

## 4. Padding

Padding is the space **inside** the border.

```css
div{
    padding: 20px;
}
```

Individual sides:

```css
padding-top: 10px;
padding-right: 20px;
padding-bottom: 10px;
padding-left: 20px;
```

Shortcut:

```css
padding: 10px 20px;
```

---

## 5. Margin

Margin is the space **outside** the border.

```css
div{
    margin: 20px;
}
```

Individual sides:

```css
margin-top: 10px;
margin-right: 20px;
margin-bottom: 10px;
margin-left: 20px;
```

Shortcut:

```css
margin: 10px 20px;
```

---

## 6. CSS Box Model

Every HTML element is a rectangular box.

The box model consists of:

```
Margin
 └── Border
      └── Padding
            └── Content
```

Example:

```css
div{
    width:200px;
    padding:20px;
    border:2px solid black;
    margin:15px;
}
```

---

## 7. Border

The border surrounds the padding.

```css
border: 2px solid black;
```

Border styles:

- solid
- dashed
- dotted
- double
- groove

Example:

```css
border:3px dashed red;
```

---

## 8. Border Radius

Rounds the corners of an element.

```css
border-radius:10px;
```

Circle:

```css
border-radius:50%;
```

---

## 9. Box Sizing

Controls how width and height are calculated.

### content-box (Default)

```css
box-sizing: content-box;
```

### border-box (Recommended)

```css
box-sizing: border-box;
```

Example:

```css
*{
    box-sizing:border-box;
}
```

---

## 10. Font Weight

Controls the thickness of text.

```css
font-weight:bold;
```

Values:

```css
font-weight:100;
font-weight:400;
font-weight:700;
font-weight:900;
```

---

## 11. Images in CSS

Control image size using CSS.

```css
img{
    width:300px;
    height:auto;
}
```

Rounded image:

```css
img{
    border-radius:50%;
}
```

Responsive image:

```css
img{
    width:100%;
    height:auto;
}
```

---

## 12. Overflow

Controls what happens when content exceeds the element size.

```css
overflow:visible;
overflow:hidden;
overflow:scroll;
overflow:auto;
```

Example:

```css
div{
    width:200px;
    height:100px;
    overflow:auto;
}
```

---

## 13. Display: Flex and Grid

### Flexbox

Used for arranging items in one direction (row or column).

```css
.container{
    display:flex;
}
```

Example:

```css
.container{
    display:flex;
    justify-content:center;
    align-items:center;
    gap:20px;
}
```

Common Properties

- flex-direction
- justify-content
- align-items
- flex-wrap
- gap

---

### Grid

Used for arranging items in rows and columns.

```css
.container{
    display:grid;
}
```

Example:

```css
.container{
    display:grid;
    grid-template-columns:1fr 1fr 1fr;
}
```

---

## 14. Grid Template

Defines the number and size of columns and rows.

Columns:

```css
grid-template-columns:1fr 1fr 1fr;
```

Rows:

```css
grid-template-rows:100px 100px;
```

Example:

```css
.container{
    display:grid;
    grid-template-columns:200px 200px 200px;
    gap:20px;
}
```

Using `repeat()`:

```css
grid-template-columns:repeat(3, 1fr);
```

This creates three equal-width columns.

---

## Summary

Today you learned:

- ✅ CSS naming conventions
- ✅ Internal (Embedded) CSS
- ✅ Font style
- ✅ Padding
- ✅ Margin
- ✅ CSS Box Model
- ✅ Border
- ✅ Border Radius
- ✅ Box Sizing
- ✅ Font Weight
- ✅ Styling Images
- ✅ Overflow
- ✅ Flexbox
- ✅ CSS Grid
- ✅ Grid Template
