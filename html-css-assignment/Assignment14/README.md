# Assignment 14: CSS Grid Layouts

## 1. Experiment Title

CSS Grid Layouts in CSS.

## 2. Aim

To make a grid with equal columns, a responsive gallery and a layout with named areas.

## 3. Software / Tools Required

- Programming Language: HTML and CSS
- Web Browser: Google Chrome / Microsoft Edge
- IDE: Visual Studio Code

## 4. Theory

CSS Grid is a layout method that arranges items in rows and columns.

The following concepts are used in this experiment:

1. **Grid Container:** `display: grid` turns an element into a grid container. `grid-template-columns` sets the columns and `gap` sets the space between the items.
2. **fr Unit:** `fr` is a fraction of the free space. `1fr 1fr 1fr` makes three equal columns.
3. **Responsive Gallery:** `repeat(auto-fill, minmax(150px, 1fr))` fits as many columns of at least 150px as possible, so more boxes fit in a row when the window is wider.
4. **Named Areas:** `grid-template-areas` names the parts of the layout, and `grid-area` places an element in a named area.

## 5. Algorithm / Procedure

### Question 1: Grid with Three Columns

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add a `<div>` with the class "grid".
4. Inside it, add six `<div>` boxes with the numbers 1 to 6.
5. In the CSS file, set `.grid` to `display: grid`.
6. Set `grid-template-columns: 1fr 1fr 1fr` for three equal columns and `gap: 12px`.
7. Style the `.box` with a background colour and padding.
8. Link the CSS file `task1.css` and stop the program.

### Question 2: Responsive Gallery

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add an `<h1>` heading "Club Photo Gallery".
4. Add a `<div>` with the class "gallery" and six boxes labelled Photo 1 to Photo 6.
5. In the CSS file, set `.gallery` to `display: grid`.
6. Set `grid-template-columns: repeat(auto-fill, minmax(150px, 1fr))` and `gap: 10px`.
7. Link the CSS file `task2.css` and stop the program.

### Question 3: Layout with Named Areas

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add a `<div>` with the class "layout" and four `<div>` elements inside it: header, sidebar, main and footer.
4. In the CSS file, set `.layout` to `display: grid` with `grid-template-columns: 200px 1fr`.
5. Set `grid-template-areas` so that the header and the footer go across both columns, the sidebar is on the left and the main area is on the right.
6. Give each element its `grid-area` name and a background colour.
7. Link the CSS file `task3.css` and stop the program.

## 6. Program / Queries / Commands

### Question 1: Grid with Three Columns

**task1.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 14 - Task 1 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grid First</title>
    <link rel="stylesheet" href="task1.css">
</head>
<body>
    <div class="grid">
        <div class="box">1</div>
        <div class="box">2</div>
        <div class="box">3</div>
        <div class="box">4</div>
        <div class="box">5</div>
        <div class="box">6</div>
    </div>
</body>
</html>
```

**task1.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 14 - Task 1 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

.grid {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    gap: 12px;
}

.box {
    background-color: #457b9d;
    color: white;
    padding: 30px;
    text-align: center;
    font-size: 24px;
}
```

### Question 2: Responsive Gallery

**task2.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 14 - Task 2 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gallery</title>
    <link rel="stylesheet" href="task2.css">
</head>
<body>
    <h1>Club Photo Gallery</h1>
    <div class="gallery">
        <div class="photo">Photo 1</div>
        <div class="photo">Photo 2</div>
        <div class="photo">Photo 3</div>
        <div class="photo">Photo 4</div>
        <div class="photo">Photo 5</div>
        <div class="photo">Photo 6</div>
    </div>
</body>
</html>
```

**task2.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 14 - Task 2 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

.gallery {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
    gap: 10px;
}

.photo {
    background-color: #a8dadc;
    padding: 40px 10px;
    text-align: center;
    border: 1px solid #1d3557;
}
```

### Question 3: Layout with Named Areas

**task3.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 14 - Task 3 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dashboard Areas</title>
    <link rel="stylesheet" href="task3.css">
</head>
<body>
    <div class="layout">
        <div class="header">Header</div>
        <div class="sidebar">Sidebar</div>
        <div class="main">Main</div>
        <div class="footer">Footer</div>
    </div>
</body>
</html>
```

**task3.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 14 - Task 3 */

body {
    font-family: Arial, sans-serif;
    margin: 10px;
}

.layout {
    display: grid;
    grid-template-columns: 200px 1fr;
    grid-template-areas:
        "header header"
        "sidebar main"
        "footer footer";
    gap: 10px;
}

.layout > div {
    padding: 20px;
    color: white;
}

.header {
    grid-area: header;
    background-color: #1d3557;
}

.sidebar {
    grid-area: sidebar;
    background-color: #457b9d;
    min-height: 200px;
}

.main {
    grid-area: main;
    background-color: #2a9d8f;
}

.footer {
    grid-area: footer;
    background-color: #e63946;
}
```

## 7. Input

The following values are used in the experiment:

### Question 1:

- Six boxes numbered 1 to 6
- Three equal columns and `gap` = 12px

### Question 2:

- Six boxes labelled Photo 1 to Photo 6
- Columns = `repeat(auto-fill, minmax(150px, 1fr))`, `gap` = 10px

### Question 3:

- Columns = 200px and 1fr
- Areas = header, sidebar, main, footer

## 8. Output

### Question 1:

Open `task1.html` in a browser. The page shows six boxes in two rows of three, with small gaps between them.

### Question 2:

Open `task2.html` in a browser and change the width of the window. As the window gets wider, more boxes fit in each row.

### Question 3:

Open `task3.html` in a browser. The page shows a header across the top, a sidebar on the left, a main area on the right and a footer at the bottom.

---

**Result:** All three tasks were written to demonstrate a grid with equal columns, a responsive gallery with `auto-fill` and `minmax()`, and a layout made with named grid areas.
