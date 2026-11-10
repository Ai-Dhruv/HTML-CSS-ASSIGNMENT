# Assignment 11: Units and CSS Variables

## 1. Experiment Title

CSS Units and CSS Variables in CSS.

## 2. Aim

To use CSS units (`px`, `%` and `rem`) and to store colours and spacing in CSS variables.

## 3. Software / Tools Required

- Programming Language: HTML and CSS
- Web Browser: Google Chrome / Microsoft Edge
- IDE: Visual Studio Code

## 4. Theory

CSS units set the size of elements and text, and CSS variables store values that can be reused in many places.

The following concepts are used in this experiment:

1. **Absolute Unit:** `px` (pixel) is a fixed size, such as `width: 200px`.
2. **Relative Units:** `%` is a part of the size of the parent element. `rem` is relative to the font size of the page, so `1.5rem` is one and a half times the normal font size.
3. **CSS Variables:** A variable is defined with two dashes, such as `--main-color: #1d3557;`, usually inside `:root`. It is used with `var(--main-color)`.
4. **Design Tokens:** Colours, font sizes and spacing values stored as variables are called design tokens. Changing one variable changes the whole page.

## 5. Algorithm / Procedure

### Question 1: CSS Units

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add a `<div>` with the class "box-fixed".
4. Add a `<div>` with the class "box-half".
5. Add a `<p>` paragraph with some text.
6. In the CSS file, set `.box-fixed` to `width: 200px` and `height: 40px` with a background colour.
7. Set `.box-half` to `width: 50%` and `height: 40px` with a background colour.
8. Set the paragraph `font-size` to `1.5rem`.
9. Link the CSS file `task1.css` and stop the program.

### Question 2: CSS Variables

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add an `<h1>` heading and a `<p>` paragraph.
4. In the CSS file, define `--main-color` as #1d3557, `--accent-color` as #e63946 and `--page-padding` as 20px inside `:root`.
5. Use `var(--main-color)` and `var(--page-padding)` for the colour and the padding of the `body`.
6. Use `var(--accent-color)` for the colour of the `h1`.
7. Link the CSS file `task2.css` and stop the program.

### Question 3: Design Tokens in a CSS File

1. Start the program.
2. In the CSS file, define the variables `--primary-color` (#1d3557), `--accent-color` (#e63946), `--heading-size` (2rem) and `--spacing` (16px) inside `:root`.
3. Use `--primary-color` for the colour of the `body` and `--spacing` for its padding.
4. Use `--accent-color` for the colour of the `h1` and `--heading-size` for its font size.
5. Create `task3.html` with an `<h1>` heading and a `<p>` paragraph, and link `task3.css`.
6. Stop the program.

## 6. Program / Queries / Commands

### Question 1: CSS Units

**task1.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 11 - Task 1 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Units</title>
    <link rel="stylesheet" href="task1.css">
</head>
<body>
    <div class="box-fixed"></div>
    <br>
    <div class="box-half"></div>
    <p>This text has a font size of 1.5rem.</p>
</body>
</html>
```

**task1.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 11 - Task 1 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

.box-fixed {
    width: 200px;
    height: 40px;
    background-color: #457b9d;
}

.box-half {
    width: 50%;
    height: 40px;
    background-color: #e63946;
}

p {
    font-size: 1.5rem;
}
```

### Question 2: CSS Variables

**task2.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 11 - Task 2 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Variables</title>
    <link rel="stylesheet" href="task2.css">
</head>
<body>
    <h1>CSS Variables</h1>
    <p>The heading uses the accent colour and this text uses the main colour.</p>
</body>
</html>
```

**task2.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 11 - Task 2 */

/* The variables are defined in :root so that the whole page can use them */
:root {
    --main-color: #1d3557;
    --accent-color: #e63946;
    --page-padding: 20px;
}

body {
    font-family: Arial, sans-serif;
    color: var(--main-color);
    padding: var(--page-padding);
}

h1 {
    color: var(--accent-color);
}
```

### Question 3: Design Tokens in a CSS File

**task3.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 11 - Task 3 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tokens</title>
    <link rel="stylesheet" href="task3.css">
</head>
<body>
    <h1>Design Tokens</h1>
    <p>The colours, the heading size and the spacing come from the variables in the CSS file.</p>
</body>
</html>
```

**task3.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 11 - Task 3 */

/* Design tokens: values that are used again and again */
:root {
    --primary-color: #1d3557;
    --accent-color: #e63946;
    --heading-size: 2rem;
    --spacing: 16px;
}

body {
    font-family: Arial, sans-serif;
    color: var(--primary-color);
    padding: var(--spacing);
}

h1 {
    color: var(--accent-color);
    font-size: var(--heading-size);
}
```

**Note:** The assignment names this file `tokens.css`. In this project it is saved as `task3.css`.

## 7. Input

The following values are used in the experiment:

### Question 1:

- Box 1 = 200px wide and 40px high
- Box 2 = 50% wide and 40px high
- Paragraph font size = 1.5rem

### Question 2:

- `--main-color` = #1d3557
- `--accent-color` = #e63946
- `--page-padding` = 20px

### Question 3:

- `--primary-color` = #1d3557
- `--accent-color` = #e63946
- `--heading-size` = 2rem
- `--spacing` = 16px

## 8. Output

### Question 1:

Open `task1.html` in a browser. The page shows a 200 pixel wide box, a box that is half the width of the window, and larger text.

### Question 2:

Open `task2.html` in a browser. The heading uses the accent (red) colour and the paragraph text uses the main (dark blue) colour.

### Question 3:

Open `task3.html` in a browser. The CSS file sets the colours, the heading size and the spacing of the page.

---

**Result:** All three tasks were written to demonstrate the units `px`, `%` and `rem`, and CSS variables defined in `:root` and used with `var()`.
