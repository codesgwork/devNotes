CSS selectors are patterns used to select and apply styles to HTML elements. Selectors target elements based on attributes like class, ID, or element type. Here's a breakdown of the most common CSS selectors with examples:

### 1. **Element Selector**
The element selector selects all instances of a particular HTML element.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <style>
        p {
            color: blue;
        }
    </style>
</head>
<body>
    <p>This is a paragraph.</p>
    <p>This is another paragraph.</p>
</body>
</html>
```
In this example, both `<p>` elements will have blue text.

---

### 2. **ID Selector**
The ID selector uses the `#` symbol followed by the element's ID to select and style that specific element.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <style>
        #unique {
            color: red;
        }
    </style>
</head>
<body>
    <p id="unique">This paragraph has a unique style.</p>
    <p>This is a normal paragraph.</p>
</body>
</html>
```
Only the `<p>` with `id="unique"` will have red text.

---

### 3. **Class Selector**
The class selector uses a `.` followed by the class name to select all elements with that class.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <style>
        .highlight {
            background-color: yellow;
        }
    </style>
</head>
<body>
    <p class="highlight">This paragraph is highlighted.</p>
    <p>This paragraph is not highlighted.</p>
    <p class="highlight">This is another highlighted paragraph.</p>
</body>
</html>
```
Both paragraphs with `class="highlight"` will have a yellow background.

---

### 4. **Universal Selector**
The universal selector (`*`) applies styles to all elements on the page.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <style>
        * {
            font-family: Arial, sans-serif;
        }
    </style>
</head>
<body>
    <h1>This is a heading</h1>
    <p>This is a paragraph.</p>
</body>
</html>
```
All text on the page will use the Arial font.

---

### 5. **Group Selector**
The group selector allows you to select multiple elements and apply the same styles to them.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <style>
        h1, p {
            color: green;
        }
    </style>
</head>
<body>
    <h1>This is a heading</h1>
    <p>This is a paragraph.</p>
</body>
</html>
```
Both the `<h1>` and `<p>` elements will have green text.

---

### 6. **Descendant Selector**
The descendant selector targets elements that are descendants (children, grandchildren, etc.) of a specified element.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <style>
        div p {
            color: purple;
        }
    </style>
</head>
<body>
    <div>
        <p>This paragraph is inside a div and will be purple.</p>
    </div>
    <p>This paragraph is outside the div and will not be purple.</p>
</body>
</html>
```
Only the `<p>` inside the `<div>` will have purple text.

---

### 7. **Child Selector**
The child selector (`>`) selects only direct children of an element.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <style>
        div > p {
            color: orange;
        }
    </style>
</head>
<body>
    <div>
        <p>This paragraph is a direct child of the div and will be orange.</p>
        <div>
            <p>This paragraph is not a direct child, so it will not be orange.</p>
        </div>
    </div>
</body>
</html>
```
Only the direct child `<p>` of the `<div>` will be orange.

---

### 8. **Attribute Selector**
The attribute selector targets elements based on their attributes.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <style>
        a[href="https://www.example.com"] {
            color: red;
        }
    </style>
</head>
<body>
    <a href="https://www.example.com">This link points to example.com and will be red.</a>
    <a href="https://www.another.com">This link points to another.com and will not be red.</a>
</body>
</html>
```
Only the link with `href="https://www.example.com"` will be red.

---

### 9. **Pseudo-class Selector**
Pseudo-classes select elements based on their state, such as `:hover`, `:focus`, `:nth-child()`, etc.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <style>
        a:hover {
            color: green;
        }
    </style>
</head>
<body>
    <a href="#">Hover over this link to change its color.</a>
</body>
</html>
```
When you hover over the link, its color will change to green.

---

### 10. **Pseudo-element Selector**
Pseudo-elements style specific parts of an element, like `::before`, `::after`, or the first letter/line.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <style>
        p::first-letter {
            font-size: 200%;
            color: red;
        }
    </style>
</head>
<body>
    <p>This paragraph's first letter will be larger and red.</p>
</body>
</html>
```
The first letter of the paragraph will be larger and red.

---

These are some of the fundamental CSS selectors. By combining them, you can create powerful and flexible styles for your website!