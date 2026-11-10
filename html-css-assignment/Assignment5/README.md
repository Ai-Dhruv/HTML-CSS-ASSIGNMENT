# Assignment 5: Links and Images

## 1. Experiment Title

Links and Images in HTML.

## 2. Aim

To link two pages together using the `<a>` tag and to add a picture with the `<img>` tag and alt text.

## 3. Software / Tools Required

- Programming Language: HTML and CSS
- Web Browser: Google Chrome / Microsoft Edge
- IDE: Visual Studio Code

## 4. Theory

Links connect web pages with each other, and images make a page more attractive.

The following concepts are used in this experiment:

1. **Link:** The `<a>` (anchor) element creates a link. The `href` attribute holds the address of the page to open.
2. **Relative Path:** A relative path such as `../Task2/task2.html` tells the browser where to find a file from the current file. `..` means one folder up.
3. **Image:** The `<img>` element shows a picture. The `src` attribute is the path of the picture file.
4. **Width and Height:** The `width` and `height` attributes set the size of the picture in pixels.
5. **alt Text:** The `alt` attribute describes the picture. It is shown if the picture cannot be loaded and it is read by screen readers.

## 5. Algorithm / Procedure

### Question 1: Home Page with a Link

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add an `<h1>` heading with the text "Welcome to My Site".
4. Add a `<p>` paragraph that contains a link to the portfolio page.
5. Write the link as `<a href="../Task2/task2.html">portfolio</a>`, so the link text is "portfolio".
6. Link the CSS file `task1.css` and stop the program.

### Question 2: Portfolio Page with a Back Link

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add an `<h1>` heading with the text "My Portfolio".
4. Add a link back to the home page using `<a href="../Task1/task1.html">`.
5. Write the link text "Go back to the home page".
6. Link the CSS file `task2.css` and stop the program.

### Question 3: Image with Alt Text

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add an `<h1>` heading.
4. Add an `<img>` tag with `src="images/photo.jpg"` (the picture is in the `images` folder).
5. Set `width="200"` and `height="200"`.
6. Write an `alt` text that describes the picture.
7. Link the CSS file `task3.css` and stop the program.

## 6. Program / Queries / Commands

### Question 1: Home Page with a Link

**task1.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 5 - Task 1 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home</title>
    <link rel="stylesheet" href="task1.css">
</head>
<body>
    <h1>Welcome to My Site</h1>
    <p>Please visit my <a href="../Task2/task2.html">portfolio</a>.</p>
</body>
</html>
```

**task1.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 5 - Task 1 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

a {
    color: #1d3557;
}

a:hover {
    color: #e63946;
}
```

**Note:** In this project every page is named `taskN.html`, so the portfolio page of this assignment is `Task2/task2.html`. The link points to it with a relative path.

### Question 2: Portfolio Page with a Back Link

**task2.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 5 - Task 2 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio</title>
    <link rel="stylesheet" href="task2.css">
</head>
<body>
    <h1>My Portfolio</h1>
    <p><a href="../Task1/task1.html">Go back to the home page</a></p>
</body>
</html>
```

**task2.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 5 - Task 2 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

a {
    color: #1d3557;
}

a:hover {
    color: #e63946;
}
```

### Question 3: Image with Alt Text

**task3.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 5 - Task 3 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio Image</title>
    <link rel="stylesheet" href="task3.css">
</head>
<body>
    <h1>My Picture</h1>
    <img src="images/photo.jpg" width="200" height="200" alt="A green hill under a bright sun with a blue sky">
</body>
</html>
```

**task3.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 5 - Task 3 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

img {
    border: 3px solid #1d3557;
}
```

**Note:** The assignment says to use the file name given by your instructor. This project uses `images/photo.jpg`, which is a sample picture. Replace it with your instructor's file and change the `src` and `alt` if needed.

## 7. Input

The following values are used in the experiment:

### Question 1:

- Link text = "portfolio"
- Link target = the portfolio page (`task2.html` in the `Task2` folder)

### Question 2:

- Link text = "Go back to the home page"
- Link target = the home page (`task1.html` in the `Task1` folder)

### Question 3:

- Picture file = `images/photo.jpg`
- `width` = 200 and `height` = 200

## 8. Output

### Question 1:

Open `task1.html` in a browser. Clicking the word "portfolio" opens the portfolio page.

### Question 2:

Open `task2.html` in a browser. Clicking the link goes back to the home page.

### Question 3:

Open `task3.html` in a browser. A 200 by 200 picture is shown under the heading. If the picture is missing, the alt text is shown instead.

---

**Result:** All three HTML pages were written to demonstrate links between pages, and an image with width, height and alt text.
