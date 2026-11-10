# Assignment 13: Flexbox Layouts

## 1. Experiment Title

Flexbox Layouts in CSS.

## 2. Aim

To lay out a navigation bar, centred cards and cards that wrap, using Flexbox.

## 3. Software / Tools Required

- Programming Language: HTML and CSS
- Web Browser: Google Chrome / Microsoft Edge
- IDE: Visual Studio Code

## 4. Theory

Flexbox is a CSS layout method that arranges items in a row or a column inside a container.

The following concepts are used in this experiment:

1. **Flex Container:** `display: flex` turns an element into a flex container. Its children (flex items) are placed side by side in a row.
2. **Alignment:** `justify-content` aligns the items along the main axis (left to right) and `align-items` aligns them along the cross axis (top to bottom).
3. **Wrapping:** By default the items stay in one row. `flex-wrap: wrap` lets the items move to a new row when there is not enough space.
4. **gap:** The `gap` property sets the space between flex items.

## 5. Algorithm / Procedure

### Question 1: Navigation Bar

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add a `<nav>` element.
4. Inside it, add four links: Home, About, Events and Contact.
5. In the CSS file, set `nav` to `display: flex` with a dark background colour.
6. Make the link text white and add padding to each link.
7. Link the CSS file `task1.css` and stop the program.

### Question 2: Centred Cards

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add a `<div>` with the class "row".
4. Inside it, add three `<div>` cards with the class "card".
5. In each card, add an `<h3>` heading (Starter, Standard, Premium) and a `<p>` paragraph with the price (199, 349, 499).
6. In the CSS file, set `.row` to `display: flex`, `justify-content: center` and `align-items: center`, and give it a fixed height.
7. Style the `.card` with a width, padding, border and background colour.
8. Link the CSS file `task2.css` and stop the program.

### Question 3: Cards that Wrap

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add an `<h1>` heading "Stationery Shop".
4. Add a `<div>` with the class "row" and four cards inside it: Notebook (60), Pen (15), Bag (350) and Book (120).
5. In the CSS file, set `.row` to `display: flex`, `flex-wrap: wrap` and a `gap`.
6. Give each `.card` a fixed width (with `box-sizing: border-box`), padding, border and background colour.
7. Link the CSS file `task3.css` and stop the program.

## 6. Program / Queries / Commands

### Question 1: Navigation Bar

**task1.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 13 - Task 1 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Navigation Bar</title>
    <link rel="stylesheet" href="task1.css">
</head>
<body>
    <nav>
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="#">Events</a>
        <a href="#">Contact</a>
    </nav>
</body>
</html>
```

**task1.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 13 - Task 1 */

body {
    font-family: Arial, sans-serif;
    margin: 0;
}

nav {
    display: flex;
    background-color: #222222;
}

nav a {
    color: white;
    text-decoration: none;
    padding: 15px 20px;
}

nav a:hover {
    background-color: #555555;
}
```

### Question 2: Centred Cards

**task2.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 13 - Task 2 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Centred Cards</title>
    <link rel="stylesheet" href="task2.css">
</head>
<body>
    <div class="row">
        <div class="card">
            <h3>Starter</h3>
            <p>Price: 199</p>
        </div>
        <div class="card">
            <h3>Standard</h3>
            <p>Price: 349</p>
        </div>
        <div class="card">
            <h3>Premium</h3>
            <p>Price: 499</p>
        </div>
    </div>
</body>
</html>
```

**task2.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 13 - Task 2 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

.row {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 20px;
    height: 250px;
    border: 2px dashed #999999;
}

.card {
    width: 150px;
    padding: 15px;
    text-align: center;
    background-color: #f1faee;
    border: 2px solid #1d3557;
    border-radius: 10px;
}
```

### Question 3: Cards that Wrap

**task3.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 13 - Task 3 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wrapping Cards</title>
    <link rel="stylesheet" href="task3.css">
</head>
<body>
    <h1>Stationery Shop</h1>
    <div class="row">
        <div class="card">
            <h3>Notebook</h3>
            <p>Price: 60</p>
        </div>
        <div class="card">
            <h3>Pen</h3>
            <p>Price: 15</p>
        </div>
        <div class="card">
            <h3>Bag</h3>
            <p>Price: 350</p>
        </div>
        <div class="card">
            <h3>Book</h3>
            <p>Price: 120</p>
        </div>
    </div>
</body>
</html>
```

**task3.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 13 - Task 3 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

.row {
    display: flex;
    flex-wrap: wrap;
    gap: 15px;
}

.card {
    box-sizing: border-box;
    width: 200px;
    padding: 15px;
    text-align: center;
    background-color: #f1faee;
    border: 2px solid #1d3557;
    border-radius: 10px;
}
```

## 7. Input

The following values are used in the experiment:

### Question 1:

- Links = Home, About, Events, Contact

### Question 2:

- Cards = Starter (199), Standard (349), Premium (499)

### Question 3:

- Cards = Notebook (60), Pen (15), Bag (350), Book (120)

## 8. Output

### Question 1:

Open `task1.html` in a browser. The page shows a dark bar with four white links side by side.

### Question 2:

Open `task2.html` in a browser. The three cards are in one row and are centred both horizontally and vertically inside the dashed row.

### Question 3:

Open `task3.html` in a browser and make the window narrower. On a narrow window the cards wrap onto new rows.

---

**Result:** All three tasks were written to demonstrate a Flexbox navigation bar, cards centred with `justify-content` and `align-items`, and cards that wrap with `flex-wrap`.
