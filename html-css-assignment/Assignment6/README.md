# Assignment 6: Types of HTML Lists

## 1. Experiment Title

Types of Lists (Unordered, Ordered, Nested and Description) in HTML.

## 2. Aim

To make a bulleted list, a numbered list with a nested list, and a description list.

## 3. Software / Tools Required

- Programming Language: HTML and CSS
- Web Browser: Google Chrome / Microsoft Edge
- IDE: Visual Studio Code

## 4. Theory

Lists are used to show a group of related items in a clear way.

The following concepts are used in this experiment:

1. **Unordered List:** The `<ul>` element makes a bulleted list. Each item is written inside `<li>`.
2. **Ordered List:** The `<ol>` element makes a numbered list. Each item is written inside `<li>`.
3. **Nested List:** A list placed inside a list item of another list is called a nested list.
4. **Description List:** The `<dl>` element makes a description list. Each term is written in `<dt>` and its description in `<dd>`.

## 5. Algorithm / Procedure

### Question 1: Unordered List

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add an `<h1>` heading with the text "Shopping List".
4. Add a `<ul>` element.
5. Add three `<li>` items inside it: Notebook, Pen and Bag.
6. Link the CSS file `task1.css` and stop the program.

### Question 2: Ordered List with a Nested List

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add an `<h1>` heading with the text "Canteen Menu".
4. Add an `<ol>` element with two `<li>` items: Samosa and Sandwich.
5. Inside the Sandwich item, add another `<ol>` with two `<li>` items: Cheese and Vegetable.
6. Link the CSS file `task2.css` and stop the program.

### Question 3: Description List

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add an `<h1>` heading.
4. Add a `<dl>` element.
5. Add the first question inside a `<dt>` and its answer inside a `<dd>`.
6. Add the second question inside a `<dt>` and its answer inside a `<dd>`.
7. Link the CSS file `task3.css` and stop the program.

## 6. Program / Queries / Commands

### Question 1: Unordered List

**task1.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 6 - Task 1 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shopping List</title>
    <link rel="stylesheet" href="task1.css">
</head>
<body>
    <h1>Shopping List</h1>
    <ul>
        <li>Notebook</li>
        <li>Pen</li>
        <li>Bag</li>
    </ul>
</body>
</html>
```

**task1.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 6 - Task 1 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

h1 {
    color: #1d3557;
}
```

### Question 2: Ordered List with a Nested List

**task2.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 6 - Task 2 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Canteen Menu</title>
    <link rel="stylesheet" href="task2.css">
</head>
<body>
    <h1>Canteen Menu</h1>
    <ol>
        <li>Samosa</li>
        <li>Sandwich
            <ol>
                <li>Cheese</li>
                <li>Vegetable</li>
            </ol>
        </li>
    </ol>
</body>
</html>
```

**task2.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 6 - Task 2 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

h1 {
    color: #1d3557;
}
```

### Question 3: Description List

**task3.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 6 - Task 3 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FAQ</title>
    <link rel="stylesheet" href="task3.css">
</head>
<body>
    <h1>Library FAQ</h1>
    <dl>
        <dt>How many books can I borrow?</dt>
        <dd>You can borrow up to three books at a time.</dd>

        <dt>Is the library open on Sunday?</dt>
        <dd>No, the library is closed on Sunday.</dd>
    </dl>
</body>
</html>
```

**task3.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 6 - Task 3 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

dt {
    font-weight: bold;
    margin-top: 12px;
}

dd {
    margin-left: 25px;
}
```

## 7. Input

The following values are used in the experiment:

### Question 1:

- Items = Notebook, Pen, Bag

### Question 2:

- Main items = Samosa, Sandwich
- Nested items under Sandwich = Cheese, Vegetable

### Question 3:

- Question 1 = "How many books can I borrow?"
- Question 2 = "Is the library open on Sunday?"
- The answers are sample text

## 8. Output

### Question 1:

Open `task1.html` in a browser. The page shows the heading "Shopping List" and three bullet points.

### Question 2:

Open `task2.html` in a browser. The page shows two numbered items, and a smaller numbered list (Cheese, Vegetable) under the second one.

### Question 3:

Open `task3.html` in a browser. The page shows two questions, each followed by its answer.

---

**Result:** All three HTML pages were written to demonstrate an unordered list, an ordered list with a nested list, and a description list.
