# Assignment 12: Box Model, Cards and Scrolling

## 1. Experiment Title

Box Model, Cards and Scrolling in CSS.

## 2. Aim

To compare the `box-sizing` types, to style a card, and to make a box scroll.

## 3. Software / Tools Required

- Programming Language: HTML and CSS
- Web Browser: Google Chrome / Microsoft Edge
- IDE: Visual Studio Code

## 4. Theory

Every HTML element is a rectangular box made of content, padding, border and margin.

The following concepts are used in this experiment:

1. **Box Model:** The box model has four parts: content, `padding` (space inside the border), `border` and `margin` (space outside the border).
2. **box-sizing:** With `content-box` the `width` is only the content, so padding and border are added to it. With `border-box` the `width` includes the padding and the border.
3. **Card:** A card is a box with a background colour, a border, rounded corners (`border-radius`) and padding that holds some related content.
4. **overflow:** `overflow: auto` adds a scroll bar when the content is larger than the box.

## 5. Algorithm / Procedure

### Question 1: content-box and border-box

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add two `<div>` boxes: one with the class "content-box" and one with the class "border-box".
4. In the CSS file, give both boxes `width: 200px`, `padding: 20px` and `border: 5px solid`.
5. Set `box-sizing: content-box` for the first box.
6. Set `box-sizing: border-box` for the second box.
7. Link the CSS file `task1.css` and stop the program.

### Question 2: Card

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add a `<div>` with the class "card".
4. Inside the card, add an `<h3>` heading and a `<p>` paragraph.
5. In the CSS file, give `.card` a background colour, `border: 2px solid`, `border-radius: 12px` and `padding: 16px`.
6. Link the CSS file `task2.css` and stop the program.

### Question 3: Scrolling Box

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add a `<div>` with the class "scroll-box".
4. Inside it, add five `<p>` paragraphs: Line 1 to Line 5.
5. In the CSS file, set `.scroll-box` to `height: 120px` and `overflow: auto`.
6. Link the CSS file `task3.css` and stop the program.

## 6. Program / Queries / Commands

### Question 1: content-box and border-box

**task1.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 12 - Task 1 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Box Model</title>
    <link rel="stylesheet" href="task1.css">
</head>
<body>
    <div class="content-box">content-box</div>
    <div class="border-box">border-box</div>
</body>
</html>
```

**task1.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 12 - Task 1 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

.content-box {
    box-sizing: content-box;
    width: 200px;
    padding: 20px;
    border: 5px solid #1d3557;
    background-color: #a8dadc;
    margin-bottom: 20px;
}

.border-box {
    box-sizing: border-box;
    width: 200px;
    padding: 20px;
    border: 5px solid #e63946;
    background-color: #f1faee;
}
```

### Question 2: Card

**task2.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 12 - Task 2 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Card</title>
    <link rel="stylesheet" href="task2.css">
</head>
<body>
    <div class="card">
        <h3>Web Design Club</h3>
        <p>Join us every Friday to learn HTML and CSS.</p>
    </div>
</body>
</html>
```

**task2.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 12 - Task 2 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

.card {
    background-color: #f1faee;
    border: 2px solid #1d3557;
    border-radius: 12px;
    padding: 16px;
    width: 280px;
}
```

### Question 3: Scrolling Box

**task3.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 12 - Task 3 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Scroll</title>
    <link rel="stylesheet" href="task3.css">
</head>
<body>
    <div class="scroll-box">
        <p>Line 1</p>
        <p>Line 2</p>
        <p>Line 3</p>
        <p>Line 4</p>
        <p>Line 5</p>
    </div>
</body>
</html>
```

**task3.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 12 - Task 3 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

.scroll-box {
    width: 250px;
    height: 120px;
    overflow: auto;
    border: 2px solid #1d3557;
    padding: 0 10px;
}
```

## 7. Input

The following values are used in the experiment:

### Question 1:

- Both boxes: width = 200px, padding = 20px, border = 5px
- Box 1 = `content-box`, Box 2 = `border-box`

### Question 2:

- Card border = 2px
- `border-radius` = 12px
- `padding` = 16px

### Question 3:

- Box height = 120px
- `overflow` = auto
- Five lines of text: Line 1 to Line 5

## 8. Output

### Question 1:

Open `task1.html` in a browser. The content-box box is wider (250px in total) than the border-box box (200px in total).

### Question 2:

Open `task2.html` in a browser. The page shows a card with rounded corners, a border and a coloured background.

### Question 3:

Open `task3.html` in a browser. The five lines do not fit in the 120px box, so the box shows a scroll bar and can be scrolled.

---

**Result:** All three tasks were written to demonstrate `box-sizing`, a styled card and a scrolling box using `overflow: auto`.
