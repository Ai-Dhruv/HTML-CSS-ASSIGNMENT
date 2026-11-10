# Assignment 15: Responsive Pages with Media Queries

## 1. Experiment Title

Responsive Pages with Media Queries in CSS.

## 2. Aim

To use a media query to change a layout, to make a picture scale with its box, and to set text sizes with `rem` units.

## 3. Software / Tools Required

- Programming Language: HTML and CSS
- Web Browser: Google Chrome / Microsoft Edge
- IDE: Visual Studio Code

## 4. Theory

A responsive page adjusts its layout to the size of the screen, such as a phone or a computer.

The following concepts are used in this experiment:

1. **Viewport Meta Tag:** `<meta name="viewport" content="width=device-width, initial-scale=1.0">` tells the phone browser to use the real width of the screen.
2. **Mobile-First Design:** The base styles are written for small screens (phones). A media query then adds styles for bigger screens.
3. **Media Query:** `@media (min-width: 600px) { ... }` applies the styles inside it only when the screen is 600px wide or more.
4. **Responsive Image:** `max-width: 100%` and `height: auto` make a picture shrink to fit its box and keep its shape.
5. **rem Unit:** `rem` is relative to the font size of the page, so the text sizes stay in proportion.

## 5. Algorithm / Procedure

### Question 1: Mobile-First Cards

1. Start the program.
2. Create the HTML document structure and add the viewport meta tag in the `<head>`.
3. Add a `<div>` with the class "cards" and two `<div>` cards with the class "card" inside it.
4. In each card, add an `<h2>` heading and a `<p>` paragraph.
5. In the CSS file, write the base styles for phones (the cards are stacked).
6. Add `@media (min-width: 600px)` and set `.cards` to `display: flex` so that the cards are side by side.
7. Link the CSS file `task1.css` and stop the program.

### Question 2: Responsive Image

1. Start the program.
2. Create the HTML document structure and add the viewport meta tag in the `<head>`.
3. Add an `<h1>` heading.
4. Add an `<img>` tag with `src="images/photo.jpg"` and an `alt` text.
5. In the CSS file, set the `img` to `max-width: 100%` and `height: auto`.
6. Link the CSS file `task2.css` and stop the program.

### Question 3: Responsive Text

1. Start the program.
2. Create the HTML document structure and add the viewport meta tag in the `<head>`.
3. Add an `<h1>` heading and a `<p>` paragraph.
4. In the CSS file, set the `body` font size to `1rem` and the `h1` font size to `1.5rem`.
5. Add `@media (min-width: 600px)` and set the `h1` font size to `2.5rem` inside it.
6. Link the CSS file `task3.css` and stop the program.

## 6. Program / Queries / Commands

### Question 1: Mobile-First Cards

**task1.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 15 - Task 1 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mobile First</title>
    <link rel="stylesheet" href="task1.css">
</head>
<body>
    <div class="cards">
        <div class="card">
            <h2>Card One</h2>
            <p>On a phone the cards are stacked.</p>
        </div>
        <div class="card">
            <h2>Card Two</h2>
            <p>On a wide screen the cards are side by side.</p>
        </div>
    </div>
</body>
</html>
```

**task1.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 15 - Task 1 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

/* Base styles for phones: the cards are stacked */
.card {
    background-color: #f1faee;
    border: 2px solid #1d3557;
    border-radius: 10px;
    padding: 15px;
    margin-bottom: 15px;
}

/* Screens 600px wide and up: the cards are side by side */
@media (min-width: 600px) {
    .cards {
        display: flex;
        gap: 15px;
    }

    .card {
        flex: 1;
    }
}
```

### Question 2: Responsive Image

**task2.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 15 - Task 2 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Image</title>
    <link rel="stylesheet" href="task2.css">
</head>
<body>
    <h1>Responsive Image</h1>
    <img src="images/photo.jpg" alt="A green hill under a bright sun with a blue sky">
</body>
</html>
```

**task2.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 15 - Task 2 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

img {
    max-width: 100%;
    height: auto;
}
```

**Note:** The assignment says to use the file name given by your instructor. This project uses `images/photo.jpg`, which is a sample picture. Replace it with your instructor's file and change the `src` and `alt` if needed.

### Question 3: Responsive Text

**task3.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 15 - Task 3 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Text</title>
    <link rel="stylesheet" href="task3.css">
</head>
<body>
    <h1>Responsive Text</h1>
    <p>The heading becomes larger when the window is 600px wide or more.</p>
</body>
</html>
```

**task3.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 15 - Task 3 */

body {
    font-family: Arial, sans-serif;
    font-size: 1rem;
    margin: 20px;
}

h1 {
    font-size: 1.5rem;
}

@media (min-width: 600px) {
    h1 {
        font-size: 2.5rem;
    }
}
```

## 7. Input

The following values are used in the experiment:

### Question 1:

- Two cards
- Media query = `min-width: 600px`

### Question 2:

- Picture file = `images/photo.jpg`
- `max-width` = 100% and `height` = auto

### Question 3:

- `body` = 1rem
- `h1` = 1.5rem (2.5rem when the window is 600px or wider)

## 8. Output

### Question 1:

Open `task1.html` in a browser. On a narrow window (phone) the cards are stacked. When the window is 600px wide or more, the cards sit side by side.

### Question 2:

Open `task2.html` in a browser. On a narrow window the picture shrinks to fit. On a wide window it keeps its own size.

### Question 3:

Open `task3.html` in a browser. The heading is larger when the window is 600px wide or more.

---

**Result:** All three tasks were written to demonstrate a mobile-first layout with a media query, a responsive image and text sizes in `rem` that change with a media query.
