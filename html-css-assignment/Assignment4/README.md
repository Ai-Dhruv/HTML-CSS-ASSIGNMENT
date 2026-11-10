# Assignment 4: Divs, Attributes and a Small Fix

## 1. Experiment Title

Divs, Attributes and Fixing a Broken Page in HTML.

## 2. Aim

To group parts of a page with `<div>` elements, add a `data-` attribute, and find and fix the errors in a broken HTML page.

## 3. Software / Tools Required

- Programming Language: HTML and CSS
- Web Browser: Google Chrome / Microsoft Edge
- IDE: Visual Studio Code

## 4. Theory

HTML elements can be grouped and given names so that they can be styled and found easily.

The following concepts are used in this experiment:

1. **div Element:** The `<div>` element is a block that groups other elements together.
2. **class and id:** A `class` can be used on many elements, and an `id` must be unique on a page. Both are used to select elements in CSS.
3. **data- Attribute:** A `data-` attribute stores extra information in an element. It is not shown on the page.
4. **Closing Tags:** Every opening tag such as `<h1>` or `<p>` must have a matching closing tag. A missing or wrong closing tag breaks the page structure.

## 5. Algorithm / Procedure

### Question 1: Header, Main and Footer Divs

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add a `<div>` with the class "header" and write some text in it.
4. Add a `<div>` with the class "main" and write some text in it.
5. Add a `<div>` with the class "footer" and write some text in it.
6. Link the CSS file `task1.css` and stop the program.

### Question 2: id and data- Attribute

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add a `<div>` and give it the id "profile".
4. Inside the `<div>`, add a `<p>` paragraph.
5. Give the paragraph the attribute `data-topic="hobbies"` and write some text in it.
6. Link the CSS file `task2.css` and stop the program.

### Question 3: Fix the Broken Page

1. Start the program.
2. Read the broken page and find the errors.
3. Error 1: the `<h1>` heading has no closing tag. Add `</h1>` after "Attendance Report".
4. Error 2: the first paragraph ends with `<p>` instead of `</p>`. Replace it with `</p>`.
5. Save the corrected page as `task3.html` (the fixed attendance page).
6. Link the CSS file `task3.css` and stop the program.

## 6. Program / Queries / Commands

### Question 1: Header, Main and Footer Divs

**task1.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 4 - Task 1 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Layout Page</title>
    <link rel="stylesheet" href="task1.css">
</head>
<body>
    <div class="header">This is the header.</div>
    <div class="main">This is the main content.</div>
    <div class="footer">This is the footer.</div>
</body>
</html>
```

**task1.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 4 - Task 1 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

.header {
    background-color: #1d3557;
    color: white;
    padding: 15px;
}

.main {
    background-color: #f1faee;
    padding: 40px 15px;
}

.footer {
    background-color: #457b9d;
    color: white;
    padding: 15px;
}
```

### Question 2: id and data- Attribute

**task2.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 4 - Task 2 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Attributes Page</title>
    <link rel="stylesheet" href="task2.css">
</head>
<body>
    <div id="profile">
        <p data-topic="hobbies">I like reading books and playing cricket.</p>
    </div>
</body>
</html>
```

**task2.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 4 - Task 2 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

#profile {
    border: 2px solid #1d3557;
    padding: 10px;
}
```

### Question 3: Fix the Broken Page

**task3.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 4 - Task 3 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Attendance</title>
    <link rel="stylesheet" href="task3.css">
</head>
<body>
    <h1>Attendance Report</h1>
    <p>Asha: 92%</p>
    <p>Rohan: 85%</p>
</body>
</html>
```

**task3.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 4 - Task 3 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

h1 {
    color: #1d3557;
}
```

**Note:** The broken page given in the assignment is:

```html
<!DOCTYPE html>
<html>
<head>
<title>Attendance</title>
</head>
<body>
<h1>Attendance Report
<p>Asha: 92%<p>
<p>Rohan: 85%</p>
</body>
</html>
```

## 7. Input

The following values are used in the experiment:

### Question 1:

- Three `<div>` blocks with the classes `header`, `main` and `footer`

### Question 2:

- `div` id = "profile"
- `data-topic` = "hobbies"

### Question 3:

- Broken page given in the assignment (shown below)

## 8. Output

### Question 1:

Open `task1.html` in a browser. The page shows three blocks in order: header, main and footer, each with its own colour.

### Question 2:

Open `task2.html` in a browser. The paragraph text is shown inside a box. The `data-topic` attribute is not visible on the page (it can be seen in the browser's Elements panel).

### Question 3:

Open `task3.html` in a browser. The corrected page shows the heading "Attendance Report" and two lines: "Asha: 92%" and "Rohan: 85%".

---

**Result:** All three HTML pages were written to demonstrate `<div>` blocks, the `id` and `data-` attributes, and the correction of a broken page.
