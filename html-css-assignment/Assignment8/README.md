# Assignment 8: Sign-Up Forms and Choices

## 1. Experiment Title

Sign-Up Forms and Choices in HTML.

## 2. Aim

To make labelled forms with text, email and password fields, radio buttons, a dropdown, required fields and a submit button.

## 3. Software / Tools Required

- Programming Language: HTML and CSS
- Web Browser: Google Chrome / Microsoft Edge
- IDE: Visual Studio Code

## 4. Theory

Forms are used to take input from the user on a web page.

The following concepts are used in this experiment:

1. **form Element:** The `<form>` element holds the input fields. The `method` attribute tells how the data is sent and the `action` attribute tells where it is sent.
2. **input Types:** `<input>` has different types: `text`, `email` and `password` (hides the typed characters). A radio button (`type="radio"`) allows only one choice in a group of buttons with the same `name`.
3. **label:** A `<label>` is linked to a field by matching its `for` attribute with the `id` of the field. Clicking the label then selects the field.
4. **select:** The `<select>` element makes a dropdown, and each choice is written inside `<option>`.
5. **required and placeholder:** `required` stops the form from being submitted when the field is empty. `placeholder` shows a hint inside an empty field.

## 5. Algorithm / Procedure

### Question 1: Sign-Up Form

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add a `<form>` with `method="post"` and `action="thanks.html"`.
4. Add a text field for the full name with `id="fullname"` and a `<label for="fullname">`.
5. Add an email field with `id="email"` and a `<label for="email">`.
6. Add a password field (`type="password"`) with `id="password"` and a `<label for="password">`.
7. Add a submit button.
8. Link the CSS file `task1.css` and stop the program.

### Question 2: Radio Buttons and Dropdown

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add a `<form>` element.
4. Add two radio buttons with the same `name="gender"`: Female and Male. Link each one with a `<label>`.
5. Add a `<select>` dropdown for the course.
6. Add two `<option>` items inside it: BCA and B.Tech.
7. Link the CSS file `task2.css` and stop the program.

### Question 3: Required Fields and Placeholder

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add a `<form>` element.
4. Add a full name field and add the `required` attribute and a `placeholder` to it.
5. Add an email field and add the `required` attribute to it.
6. Add a `<button type="submit">` with the text "Submit".
7. Link the CSS file `task3.css` and stop the program.

## 6. Program / Queries / Commands

### Question 1: Sign-Up Form

**task1.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 8 - Task 1 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sign Up</title>
    <link rel="stylesheet" href="task1.css">
</head>
<body>
    <h1>Sign Up</h1>
    <form method="post" action="thanks.html">
        <p>
            <label for="fullname">Full name:</label>
            <input type="text" id="fullname" name="fullname">
        </p>
        <p>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email">
        </p>
        <p>
            <label for="password">Password:</label>
            <input type="password" id="password" name="password">
        </p>
        <button type="submit">Sign Up</button>
    </form>
</body>
</html>
```

**task1.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 8 - Task 1 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

label {
    display: inline-block;
    width: 100px;
}

input {
    padding: 5px;
}
```

### Question 2: Radio Buttons and Dropdown

**task2.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 8 - Task 2 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Choices</title>
    <link rel="stylesheet" href="task2.css">
</head>
<body>
    <h1>Choices</h1>
    <form>
        <p>Gender:</p>
        <input type="radio" id="female" name="gender" value="female">
        <label for="female">Female</label>
        <input type="radio" id="male" name="gender" value="male">
        <label for="male">Male</label>

        <p>
            <label for="course">Course:</label>
            <select id="course" name="course">
                <option value="bca">BCA</option>
                <option value="btech">B.Tech</option>
            </select>
        </p>
    </form>
</body>
</html>
```

**task2.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 8 - Task 2 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

label {
    margin-right: 15px;
}

select {
    padding: 4px;
}
```

### Question 3: Required Fields and Placeholder

**task3.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 8 - Task 3 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sign Up Required</title>
    <link rel="stylesheet" href="task3.css">
</head>
<body>
    <h1>Sign Up</h1>
    <form>
        <p>
            <label for="fullname">Full name:</label>
            <input type="text" id="fullname" name="fullname" placeholder="Enter your full name" required>
        </p>
        <p>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
        </p>
        <button type="submit">Submit</button>
    </form>
</body>
</html>
```

**task3.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 8 - Task 3 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

label {
    display: inline-block;
    width: 100px;
}

input {
    padding: 5px;
}

button {
    padding: 6px 16px;
}
```

## 7. Input

The following values are used in the experiment:

### Question 1:

- Fields = Full name, Email, Password
- `method` = "post" and `action` = "thanks.html" (the file `thanks.html` is not needed)

### Question 2:

- Gender choices = Female, Male
- Course choices = BCA, B.Tech

### Question 3:

- Full name field with placeholder "Enter your full name"
- Email field
- Both fields are `required`

## 8. Output

### Question 1:

Open `task1.html` in a browser. The page shows three labelled boxes. The password box hides the characters that are typed. Clicking a label selects its box.

### Question 2:

Open `task2.html` in a browser. Only one gender can be selected at a time. The dropdown shows the two courses, BCA and B.Tech.

### Question 3:

Open `task3.html` in a browser. The name box shows the placeholder text. If a required field is left empty and Submit is clicked, the browser shows a message and does not submit the form.

---

**Result:** All three HTML pages were written to demonstrate labelled form fields, radio buttons, a dropdown, required fields and a placeholder.
