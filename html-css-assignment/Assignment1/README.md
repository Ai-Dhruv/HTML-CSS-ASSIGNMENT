# Assignment 1: Starting a Git Repository

## 1. Experiment Title

Starting a Git Repository and Saving Work with Commits in Git.

## 2. Aim

To start a Git repository for the lab folder and to save the work with commits.

## 3. Software / Tools Required

- Version Control System: Git
- Terminal: Git Bash / Command Prompt
- IDE / Editor: Visual Studio Code
- Web Browser: Google Chrome / Microsoft Edge

## 4. Theory

Git is a version control system. It saves the history of a project, so every change can be seen and recovered.

The following concepts are used in this experiment:

1. **Repository:** A repository is a project folder that Git tracks. `git init` starts a new repository.
2. **Configuration:** `git config --local` saves the user name and the user email for one repository only. `git config user.name` and `git config user.email` show the saved values.
3. **Staging and Commit:** `git status` shows the state of the files. `git add` puts a file in the staging area and `git commit -m "message"` saves a snapshot with a message.
4. **History:** `git log --oneline` shows the commits in short form, the newest one first.

## 5. Algorithm / Procedure

### Question 1: Start a Git Repository and Set the Name and Email

1. Start the program.
2. Create a folder named `html-lab` and go into it.
3. Start a Git repository with `git init`.
4. Set your name for this repository only with `git config --local user.name`.
5. Set your email for this repository only with `git config --local user.email`.
6. Show the values with `git config user.name` and `git config user.email`.
7. Stop the program.

### Question 2: Create index.html and Make the First Commit

1. Start the program.
2. Create the file `index.html` inside `html-lab` with one `<h1>` heading (see `task2.html`).
3. Run `git status` to see that `index.html` is untracked.
4. Add the file to the staging area with `git add index.html`.
5. Save it with `git commit -m "Add home page"`.
6. Stop the program.

### Question 3: Add an h2 Heading and Make the Second Commit

1. Start the program.
2. Open `index.html` and add an `<h2>` heading below the `<h1>` heading (see `task3.html`).
3. Add the changed file with `git add index.html`.
4. Save it with `git commit -m "Add next meeting heading"`.
5. Show the history with `git log --oneline`.
6. Stop the program.

## 6. Program / Queries / Commands

### Question 1: Start a Git Repository and Set the Name and Email

```bash
mkdir html-lab
cd html-lab
git init
git config --local user.name "Dhruv Saxena"
git config --local user.email "dhruv.saxena@example.com"
git config user.name
git config user.email
```

### Question 2: Create index.html and Make the First Commit

```bash
git status
git add index.html
git commit -m "Add home page"
```

**index.html** (saved as `task2.html`)

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 1 - Task 2 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Home Page</title>
</head>
<body>
    <h1>Welcome to My HTML Lab</h1>
</body>
</html>
```

### Question 3: Add an h2 Heading and Make the Second Commit

```bash
git add index.html
git commit -m "Add next meeting heading"
git log --oneline
```

**index.html** (saved as `task3.html`)

```html
<!DOCTYPE html>
<!-- Name: Dhruv Saxena | Roll No: BCS2025626 | Assignment: 1 - Task 3 -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Home Page</title>
</head>
<body>
    <h1>Welcome to My HTML Lab</h1>
    <h2>Next Meeting</h2>
</body>
</html>
```

## 7. Input

The following values are used in the experiment:

### Question 1:

- Folder name = `html-lab`
- Name = "Dhruv Saxena"
- Email = "dhruv.saxena@example.com" (replace with your own email)

### Question 2:

- File = `index.html` with one `<h1>` heading
- Commit message = "Add home page"

### Question 3:

- Added heading = `<h2>Next Meeting</h2>`
- Commit message = "Add next meeting heading"

## 8. Output

### Question 1:

```text
$ git init
Initialized empty Git repository in .../html-lab/.git/
$ git config --local user.name "Dhruv Saxena"
$ git config --local user.email "dhruv.saxena@example.com"
$ git config user.name
Dhruv Saxena
$ git config user.email
dhruv.saxena@example.com
```

*Output may differ on your computer: the commit IDs and the folder paths will be different. The `hint:` lines that Git prints about the default branch name are not shown.*

### Question 2:

```text
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	index.html

nothing added to commit but untracked files present (use "git add" to track)
$ git add index.html
$ git commit -m "Add home page"
[master (root-commit) e64b025] Add home page
 1 file changed, 12 insertions(+)
 create mode 100644 index.html
```


### Question 3:

```text
$ git add index.html
$ git commit -m "Add next meeting heading"
[master 76568ef] Add next meeting heading
 1 file changed, 2 insertions(+), 1 deletion(-)
$ git log --oneline
76568ef Add next meeting heading
e64b025 Add home page
```


---

**Result:** All three Git tasks were written to demonstrate starting a repository, setting the name and email, adding a file, and saving the work with two commits.
