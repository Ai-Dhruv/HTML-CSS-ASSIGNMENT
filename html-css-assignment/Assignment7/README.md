# Assignment 7: About Me Page

## 1. Experiment Title

About Me Page using Semantic Tags in HTML.

## 2. Aim

To build a short About Me page using semantic tags, an about section and a contact link.

## 3. Software / Tools Required

- Programming Language: HTML and CSS
- Web Browser: Google Chrome / Microsoft Edge
- IDE: Visual Studio Code

## 4. Theory

Semantic tags describe the meaning of each part of a page, which makes the page easier to read, to style and to use with screen readers.

The following concepts are used in this experiment:

1. **Semantic Tags:** `<header>`, `<nav>`, `<main>`, `<section>` and `<footer>` show the role of each part of the page.
2. **Page Links:** A link that starts with `#` jumps to the element that has the same `id` on the same page, such as `href="#about"` and `id="about"`.
3. **Email Link:** A link with `href="mailto:..."` opens the email program with the given address.
4. **Building a Page Step by Step:** The page is built in three steps. Each task adds more content to the page of the previous task.

## 5. Algorithm / Procedure

### Question 1: Header, Navigation, Main and Footer

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add a `<header>` element.
4. Inside the header, add an `<h1>` with your name.
5. Inside the header, add a `<nav>` with two links: "About" (`href="#about"`) and "Contact" (`href="#contact"`).
6. Add an empty `<main>` element and an empty `<footer>` element.
7. Link the CSS file `task1.css` and stop the program.

### Question 2: About Section

1. Start the program.
2. Start with the page of Task 1.
3. Add a `<section>` with the id "about" inside `<main>`.
4. Inside the section, add an `<h2>` heading "About me".
5. Inside the section, add a `<p>` paragraph about yourself.
6. Keep the CSS file linked as `task2.css` and stop the program.

### Question 3: Contact Footer with an Email Link

1. Start the program.
2. Start with the page of Task 2.
3. Give the `<footer>` the id "contact".
4. Inside the footer, add a `<p>` paragraph.
5. In the paragraph, add a link with `href="mailto:..."` and your email address as the link text.
6. Keep the CSS file linked as `task3.css` and stop the program.

## 6. Program / Queries / Commands

### Question 1: Header, Navigation, Main and Footer

**task1.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 7 - Task 1 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About Me</title>
    <link rel="stylesheet" href="task1.css">
</head>
<body>
    <header>
        <h1>Dhruv Saxena</h1>
        <nav>
            <a href="#about">About</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>
    <main>
    </main>

    <footer>
    </footer>
</body>
</html>
```

**task1.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 7 - Task 1 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

header {
    background-color: #1d3557;
    color: white;
    padding: 15px;
}

nav a {
    color: white;
    margin-right: 15px;
}

main {
    padding: 20px 0;
    min-height: 120px;
}

footer {
    background-color: #457b9d;
    color: white;
    padding: 15px;
}

footer a {
    color: white;
}
```

### Question 2: About Section

**task2.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 7 - Task 2 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About Me</title>
    <link rel="stylesheet" href="task2.css">
</head>
<body>
    <header>
        <h1>Dhruv Saxena</h1>
        <nav>
            <a href="#about">About</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>
    <main>
        <section id="about">
            <h2>About me</h2>
            <p>I am a first-year B.Tech student at Invertis University, Bareilly. I am learning HTML and CSS to build web pages.</p>
        </section>
    </main>

    <footer>
    </footer>
</body>
</html>
```

**task2.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 7 - Task 2 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

header {
    background-color: #1d3557;
    color: white;
    padding: 15px;
}

nav a {
    color: white;
    margin-right: 15px;
}

main {
    padding: 20px 0;
    min-height: 120px;
}

footer {
    background-color: #457b9d;
    color: white;
    padding: 15px;
}

footer a {
    color: white;
}
```

### Question 3: Contact Footer with an Email Link

**task3.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 7 - Task 3 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About Me</title>
    <link rel="stylesheet" href="task3.css">
</head>
<body>
    <header>
        <h1>Dhruv Saxena</h1>
        <nav>
            <a href="#about">About</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>
    <main>
        <section id="about">
            <h2>About me</h2>
            <p>I am a first-year B.Tech student at Invertis University, Bareilly. I am learning HTML and CSS to build web pages.</p>
        </section>
    </main>

    <footer id="contact">
        <p>Email: <a href="mailto:dhruv.saxena@example.com">dhruv.saxena@example.com</a></p>
    </footer>
</body>
</html>
```

**task3.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 7 - Task 3 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

header {
    background-color: #1d3557;
    color: white;
    padding: 15px;
}

nav a {
    color: white;
    margin-right: 15px;
}

main {
    padding: 20px 0;
    min-height: 120px;
}

footer {
    background-color: #457b9d;
    color: white;
    padding: 15px;
}

footer a {
    color: white;
}
```

**Note:** `dhruv.saxena@example.com` is a sample address. Replace it with your own email address.

## 7. Input

The following values are used in the experiment:

### Question 1:

- Name = "Dhruv Saxena"
- Links = About (`#about`) and Contact (`#contact`)

### Question 2:

- Section id = "about"
- Heading = "About me"
- One paragraph about yourself

### Question 3:

- Footer id = "contact"
- Email = dhruv.saxena@example.com (replace with your own email)

## 8. Output

### Question 1:

Open `task1.html` in a browser. The page shows the name at the top with two links. The middle and the bottom of the page are empty.

### Question 2:

Open `task2.html` in a browser. The heading "About me" and a paragraph appear under the top links. Clicking "About" jumps to this section.

### Question 3:

Open `task3.html` in a browser. The footer shows a clickable email address. Clicking "Contact" in the top navigation jumps to the footer.

---

**Result:** All three HTML pages were written step by step to demonstrate semantic tags, links to sections of the same page, and a `mailto:` link.
