# Assignment 9: Tables with Headers and Footers

## 1. Experiment Title

Tables with Headers, Footers and Scope in HTML.

## 2. Aim

To build a table with a caption, a header, rows and a footer, and to add `scope` attributes.

## 3. Software / Tools Required

- Programming Language: HTML and CSS
- Web Browser: Google Chrome / Microsoft Edge
- IDE: Visual Studio Code

## 4. Theory

Tables are used to show data in rows and columns.

The following concepts are used in this experiment:

1. **Table Elements:** `<table>` makes the table, `<tr>` makes a row, `<th>` makes a header cell and `<td>` makes a data cell.
2. **Table Sections:** `<caption>` gives the table a title. `<thead>`, `<tbody>` and `<tfoot>` group the header rows, the body rows and the footer rows.
3. **scope Attribute:** `scope="col"` tells that a header cell describes a column and `scope="row"` tells that it describes a row. It helps screen readers.
4. **Average:** The class average of the two students is calculated as: Maths = (78 + 64) / 2 = 71 and Science = (85 + 70) / 2 = 77.5.

## 5. Algorithm / Procedure

### Question 1: Marks Table

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add a `<table>` with the caption "Marks of Class A".
4. Add a `<thead>` with one row of header cells: Name, Maths, Science.
5. Add a `<tbody>` with three rows: Asha 78 85, Rohan 64 70 and Neha 91 88.
6. Link the CSS file `task1.css` and stop the program.

### Question 2: Marks Table with a Footer

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add the same table caption and header as Task 1.
4. Add a `<tbody>` with only the Asha and Rohan rows.
5. Calculate the average Maths marks: (78 + 64) / 2 = 71.
6. Calculate the average Science marks: (85 + 70) / 2 = 77.5.
7. Add a `<tfoot>` row with the cells "Class average", 71 and 77.5.
8. Link the CSS file `task2.css` and stop the program.

### Question 3: Accessible Table with Scope

1. Start the program.
2. Create the HTML document structure and set a page title.
3. Add the same table caption, header and the Asha and Rohan rows as Task 2, without the footer row.
4. Add `scope="col"` to each header cell in the `<thead>`.
5. Make each name cell a `<th>` cell and add `scope="row"` to it.
6. Link the CSS file `task3.css` and stop the program.

## 6. Program / Queries / Commands

### Question 1: Marks Table

**task1.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 9 - Task 1 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Marks</title>
    <link rel="stylesheet" href="task1.css">
</head>
<body>
    <h1>Marks Table</h1>
    <table>
        <caption>Marks of Class A</caption>
        <thead>
            <tr>
                <th>Name</th>
                <th>Maths</th>
                <th>Science</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Asha</td>
                <td>78</td>
                <td>85</td>
            </tr>
            <tr>
                <td>Rohan</td>
                <td>64</td>
                <td>70</td>
            </tr>
            <tr>
                <td>Neha</td>
                <td>91</td>
                <td>88</td>
            </tr>
        </tbody>
    </table>
</body>
</html>
```

**task1.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 9 - Task 1 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

table {
    border-collapse: collapse;
    width: 400px;
}

th, td {
    border: 1px solid #333;
    padding: 8px;
    text-align: center;
}

thead th {
    background-color: #1d3557;
    color: white;
}

tfoot td {
    background-color: #f1faee;
    font-weight: bold;
}

caption {
    font-weight: bold;
    margin-bottom: 8px;
}
```

### Question 2: Marks Table with a Footer

**task2.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 9 - Task 2 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Marks Average</title>
    <link rel="stylesheet" href="task2.css">
</head>
<body>
    <h1>Marks Table</h1>
    <table>
        <caption>Marks of Class A</caption>
        <thead>
            <tr>
                <th>Name</th>
                <th>Maths</th>
                <th>Science</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Asha</td>
                <td>78</td>
                <td>85</td>
            </tr>
            <tr>
                <td>Rohan</td>
                <td>64</td>
                <td>70</td>
            </tr>
        </tbody>
        <tfoot>
            <tr>
                <td>Class average</td>
                <td>71</td>
                <td>77.5</td>
            </tr>
        </tfoot>
    </table>
</body>
</html>
```

**task2.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 9 - Task 2 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

table {
    border-collapse: collapse;
    width: 400px;
}

th, td {
    border: 1px solid #333;
    padding: 8px;
    text-align: center;
}

thead th {
    background-color: #1d3557;
    color: white;
}

tfoot td {
    background-color: #f1faee;
    font-weight: bold;
}

caption {
    font-weight: bold;
    margin-bottom: 8px;
}
```

### Question 3: Accessible Table with Scope

**task3.html**

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 9 - Task 3 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Marks Accessible</title>
    <link rel="stylesheet" href="task3.css">
</head>
<body>
    <h1>Marks Table</h1>
    <table>
        <caption>Marks of Class A</caption>
        <thead>
            <tr>
                <th scope="col">Name</th>
                <th scope="col">Maths</th>
                <th scope="col">Science</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <th scope="row">Asha</th>
                <td>78</td>
                <td>85</td>
            </tr>
            <tr>
                <th scope="row">Rohan</th>
                <td>64</td>
                <td>70</td>
            </tr>
        </tbody>
    </table>
</body>
</html>
```

**task3.css**

```css
/* Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 9 - Task 3 */

body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 20px;
}

table {
    border-collapse: collapse;
    width: 400px;
}

th, td {
    border: 1px solid #333;
    padding: 8px;
    text-align: center;
}

thead th {
    background-color: #1d3557;
    color: white;
}

tfoot td {
    background-color: #f1faee;
    font-weight: bold;
}

caption {
    font-weight: bold;
    margin-bottom: 8px;
}
```

**Note:** The name cells are written as `<th scope="row">` cells because `scope="row"` is used on header cells. Their text is bold and centred by the CSS file like the other cells.

## 7. Input

The following values are used in the experiment:

### Question 1:

- Header = Name, Maths, Science
- Asha 78 85
- Rohan 64 70
- Neha 91 88

### Question 2:

- Asha 78 85
- Rohan 64 70
- Class average = 71 and 77.5

### Question 3:

- Asha 78 85
- Rohan 64 70

## 8. Output

### Question 1:

Open `task1.html` in a browser. The page shows a table with the caption, a header row and three student rows.

### Question 2:

Open `task2.html` in a browser. The footer row at the bottom shows "Class average" with the two averages, 71 and 77.5.

### Question 3:

Open `task3.html` in a browser. The table looks like the previous one without the footer. The header cells and the name cells carry `scope` attributes (check them in the browser's Elements panel).

---

**Result:** All three HTML pages were written to demonstrate a table with a caption, a header, a body and a footer, and the `scope` attribute.
