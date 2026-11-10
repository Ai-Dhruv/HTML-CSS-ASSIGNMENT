# Assignment 10: CSS Fundamentals

## 1. Experiment Title

CSS Fundamentals (Inline, Internal and Linked CSS) and Selectors in CSS.

## 2. Aim

To apply CSS in three ways (inline, internal and linked) and to use element, class and id selectors and text styles.

## 3. Software / Tools Required

- Programming Language: HTML and CSS
- Web Browser: Google Chrome / Microsoft Edge
- IDE: Visual Studio Code

## 4. Theory

CSS (Cascading Style Sheets) is used to change the colours, text and look of an HTML page.

The following concepts are used in this experiment:

1. **Three Ways to Add CSS:** The three ways are:
   - Inline : the `style` attribute inside a tag.
   - Internal : a `<style>` block inside the `<head>`.
   - Linked : an external `.css` file connected with `<link rel="stylesheet" href="...">`.
2. **Selectors:** An element selector such as `h1` selects all `<h1>` elements. A class selector such as `.note` selects elements with `class="note"`. An id selector such as `#title` selects the element with `id="title"`.
3. **Text Properties:** `color` sets the text colour, `font-style: italic` makes the text italic, `text-decoration: underline` underlines the text and `font-size` sets the size of the text.
4. **Background:** `background-color` sets the background colour of an element.

## 5. Algorithm / Procedure

### Question 1: Inline and Internal CSS

1. Start the program.
2. Create the HTML document structure and set a page title.
3. In the `<head>`, add a `<style>` block (internal CSS).
4. In the style block, make the `h1` colour navy.
5. In the style block, give the class `highlight` a yellow background.
6. In the `<body>`, add an `<h1>` heading.
7. Add a `<p>` paragraph with an inline style `style="color: red;"`.
8. Add a `<p>` paragraph with the class "highlight".
9. Link the CSS file `task1.css` for the general page style and stop the program.

### Question 2: CSS Rules for Selectors

1. Start the program.
2. Write a rule for all `h1` elements and set the colour to navy.
3. Write a rule for the class `.note` and set `font-style` to italic.
4. Write a rule for the id `#title` and set `text-decoration` to underline.
5. Write a rule for all `p` elements and set `font-size` to 18px and the colour to grey.
6. Use the page `task2.html` to see the rules (it links `task2.css`).
7. Stop the program.

### Question 3: Linked CSS

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Link the CSS file in the `<head>` using `<link rel="stylesheet" href="task3.css">`.
4. Add an `<h1>` heading with the id "title".
5. Add two `<p>` paragraphs with the class "note".
6. Keep `task3.css` in the same folder as the page and stop the program.

## 6. Program / Queries / Commands

### Question 1: Inline and Internal CSS

**task1.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 10 - Task 1 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Inline, Internal and Linked CSS</title>
    <!-- Linked CSS: general page style -->
    <link rel="stylesheet" href="task1.css">
    <!-- Internal CSS: written inside a style block -->
    <style>
        h1 {
            color: navy;
        }

        .highlight {
            background-color: yellow;
        }
    </style>
</head>
<body>
    <h1>CSS in Three Ways</h1>
    <!-- Inline CSS: written in the style attribute -->
    <p style="color: red;">This paragraph is red because of an inline style.</p>
    <p class="highlight">This paragraph has a yellow background because of an internal style.</p>
</body>
</html>
```

**task1.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 10 - Task 1 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}
```

### Question 2: CSS Rules for Selectors

**task2.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 10 - Task 2 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Selectors</title>
    <link rel="stylesheet" href="task2.css">
</head>
<body>
    <h1 id="title">Styling with CSS</h1>
    <p class="note">This paragraph has the class note.</p>
    <p>This is a normal paragraph.</p>
</body>
</html>
```

**task2.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 10 - Task 2 */

h1 {
    color: navy;
}

.note {
    font-style: italic;
}

#title {
    text-decoration: underline;
}

p {
    font-size: 18px;
    color: grey;
}
```

**Note:** The assignment names this file `style.css`. In this project it is saved as `task2.css`.

### Question 3: Linked CSS

**task3.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 10 - Task 3 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Linked CSS</title>
    <link rel="stylesheet" href="task3.css">
</head>
<body>
    <h1 id="title">Linked CSS Page</h1>
    <p class="note">This is the first note.</p>
    <p class="note">This is the second note.</p>
</body>
</html>
```

**task3.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 10 - Task 3 */

h1 {
    color: navy;
}

.note {
    font-style: italic;
}

#title {
    text-decoration: underline;
}

p {
    font-size: 18px;
    color: grey;
}
```

**Note:** The assignment says to link `style.css`. In this project the same rules are saved in `task3.css`, which is linked from `task3.html`.

## 7. Input

The following values are used in the experiment:

### Question 1:

- `h1` colour = navy (internal CSS)
- Class `highlight` background = yellow (internal CSS)
- Paragraph text colour = red (inline CSS)

### Question 2:

- `h1` colour = navy
- `.note` = italic
- `#title` = underlined
- `p` = 18px and grey

### Question 3:

- `h1` id = "title"
- Two paragraphs with the class "note"

## 8. Output

### Question 1:

Open `task1.html` in a browser. The page shows a navy heading, one red paragraph and one paragraph with a yellow background.

### Question 2:

Open `task2.html` in a browser. The heading is navy and underlined, the note paragraph is italic, and all paragraphs have a font size of 18px and a grey colour.

### Question 3:

Open `task3.html` in a browser. The page is styled by the linked CSS file: a navy underlined heading and two italic grey paragraphs. If the CSS file is not in the same folder, the page is not styled.

---

**Result:** All three tasks were written to demonstrate inline, internal and linked CSS, and the element, class and id selectors with text styles.
