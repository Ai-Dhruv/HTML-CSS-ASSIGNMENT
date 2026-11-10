# Assignment 3: Your First HTML Page

## 1. Experiment Title

Your First HTML Page with Headings and Text Formatting in HTML.

## 2. Aim

To write HTML pages with a document structure, a title, headings and paragraphs, and to format text using `<strong>`, `<em>` and `<br>`.

## 3. Software / Tools Required

- Programming Language: HTML and CSS
- Web Browser: Google Chrome / Microsoft Edge
- IDE: Visual Studio Code

## 4. Theory

HTML (HyperText Markup Language) is used to create the structure of a web page.

The following concepts are used in this experiment:

1. **Document Structure:** Every HTML page starts with `<!DOCTYPE html>` and has the `<html>`, `<head>` and `<body>` elements. The `<head>` holds information such as the `<title>`, and the `<body>` holds the content shown on the page.
2. **Headings:** HTML has six heading levels from `<h1>` (largest) to `<h6>` (smallest).
3. **Paragraph:** The `<p>` element is used to write a paragraph of text.
4. **Text Formatting:** `<strong>` shows important text in bold, `<em>` shows emphasised text in italics and `<br>` starts a new line inside a paragraph.
5. **CSS Link:** The `<link>` element in the `<head>` connects an HTML page with its CSS file.

## 5. Algorithm / Procedure

### Question 1: First Page with a Heading

1. Start the program.
2. Create the HTML document structure using `<!DOCTYPE html>`, `<html>`, `<head>` and `<body>`.
3. Set the page title to "My First Page" using the `<title>` tag.
4. Add one `<h1>` heading with the text "Hello, I am Asha".
5. Link the CSS file `task1.css` in the `<head>`.
6. Open the page in a browser.
7. Stop the program.

### Question 2: Headings and Paragraph

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add an `<h1>` heading with the text "Main Heading".
4. Add an `<h2>` heading with the text "Sub Heading".
5. Add an `<h3>` heading with the text "Smaller Heading".
6. Add one `<p>` paragraph below the headings.
7. Link the CSS file `task2.css` and stop the program.

### Question 3: Text Formatting

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add an `<h1>` heading.
4. Add the first `<p>` paragraph and put one word inside `<strong>` and one word inside `<em>`.
5. Add the second `<p>` paragraph and put a `<br>` tag inside it.
6. Link the CSS file `task3.css` and stop the program.

## 6. Program / Queries / Commands

### Question 1: First Page with a Heading

**task1.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 3 - Task 1 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First Page</title>
    <link rel="stylesheet" href="task1.css">
</head>
<body>
    <h1>Hello, I am Asha</h1>
</body>
</html>
```

**task1.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 3 - Task 1 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

h1 {
    color: #1d3557;
}
```

### Question 2: Headings and Paragraph

**task2.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 3 - Task 2 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Headings Page</title>
    <link rel="stylesheet" href="task2.css">
</head>
<body>
    <h1>Main Heading</h1>
    <h2>Sub Heading</h2>
    <h3>Smaller Heading</h3>
    <p>HTML has six heading levels. The <code>h1</code> heading is the largest and each next level is a little smaller.</p>
</body>
</html>
```

**task2.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 3 - Task 2 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

h1 {
    color: #1d3557;
}

h2 {
    color: #457b9d;
}

h3 {
    color: #e63946;
}
```

### Question 3: Text Formatting

**task3.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 3 - Task 3 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Text Formatting Page</title>
    <link rel="stylesheet" href="task3.css">
</head>
<body>
    <h1>Text Formatting</h1>
    <p>HTML lets us make a word <strong>important</strong> or <em>emphasised</em> inside a paragraph.</p>
    <p>This paragraph has a line break.<br>This text starts on a new line.</p>
</body>
</html>
```

**task3.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 3 - Task 3 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

strong {
    color: #e63946;
}

em {
    color: #1d3557;
}
```

## 7. Input

The following values are used in the experiment:

### Question 1:

- Page title = "My First Page"
- Heading = "Hello, I am Asha"

### Question 2:

- `h1` = "Main Heading"
- `h2` = "Sub Heading"
- `h3` = "Smaller Heading"
- One paragraph of text

### Question 3:

- Two paragraphs of text
- One word in `<strong>` and one word in `<em>`
- One `<br>` line break

## 8. Output

### Question 1:

Open `task1.html` in a browser. The browser tab shows the title "My First Page" and the page shows one large heading: "Hello, I am Asha".

### Question 2:

Open `task2.html` in a browser. The page shows three headings, each smaller than the one above, and a paragraph under them.

### Question 3:

Open `task3.html` in a browser. The word in `<strong>` looks bold and the word in `<em>` looks italic. The line break starts a new line inside the second paragraph.

---

**Result:** All three HTML pages were written to demonstrate the document structure, headings, paragraphs and text formatting, and each page is linked with its CSS file.
