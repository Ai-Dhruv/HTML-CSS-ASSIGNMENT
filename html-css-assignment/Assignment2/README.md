# Assignment 2: Pushing and Cloning a Repository

## 1. Experiment Title

Pushing and Cloning a Repository in Git.

## 2. Aim

To send the commits to a second repository on the computer and to make a copy of it with `git clone`.

## 3. Software / Tools Required

- Version Control System: Git
- Terminal: Git Bash / Command Prompt
- IDE / Editor: Visual Studio Code
- Web Browser: Google Chrome / Microsoft Edge

## 4. Theory

A remote repository is a second copy of a repository. It is used to share the work or to keep a backup.

The following concepts are used in this experiment:

1. **Bare Repository:** `git init --bare` creates a repository without a working folder. It is used as a central place to push to.
2. **Remote:** `git remote add origin <path>` saves the address of a remote repository under the name `origin`. `git remote -v` lists the remotes.
3. **Push:** `git push origin <branch>` sends the commits of a branch to the remote repository.
4. **Clone:** `git clone <repository> <folder>` makes a full copy of a repository, including its history.

## 5. Algorithm / Procedure

### Question 1: Create a Bare Repository and Add it as origin

1. Start the program.
2. Go into the `html-lab` folder.
3. Create an empty (bare) repository next to it with `git init --bare ../html-remote`.
4. Add it as the remote named `origin` with `git remote add origin ../html-remote`.
5. Show the remotes with `git remote -v`.
6. Stop the program.

### Question 2: Push the Commits to origin

1. Start the program.
2. Run `git status` to see the branch name.
3. Push the commits with `git push origin master` (use `git push origin main` if the branch is `main`).
4. Check the last line of the output, which shows the branch.
5. Stop the program.

### Question 3: Clone the Repository

1. Start the program.
2. Go up one folder from `html-lab` with `cd ..`.
3. Clone `html-remote` into a new folder with `git clone html-remote html-copy`.
4. Go into the `html-copy` folder with `cd html-copy`.
5. Show the history with `git log --oneline`.
6. Stop the program.

## 6. Program / Queries / Commands

### Question 1: Create a Bare Repository and Add it as origin

```bash
cd html-lab
git init --bare ../html-remote
git remote add origin ../html-remote
git remote -v
```

### Question 2: Push the Commits to origin

```bash
git status
git push origin master
# If git status shows 'On branch main', use: git push origin main
```

### Question 3: Clone the Repository

```bash
cd ..
git clone html-remote html-copy
cd html-copy
git log --oneline
```

## 7. Input

The following values are used in the experiment:

### Question 1:

- Remote folder = `../html-remote`
- Remote name = `origin`

### Question 2:

- Branch name = `master`
- Remote name = `origin`

### Question 3:

- Repository to clone = `html-remote`
- New folder = `html-copy`

## 8. Output

### Question 1:

```text
$ git init --bare ../html-remote
Initialized empty Git repository in .../html-remote/
$ git remote add origin ../html-remote
$ git remote -v
origin	../html-remote (fetch)
origin	../html-remote (push)
```

*Output may differ on your computer: the commit IDs and the folder paths will be different. The `hint:` lines that Git prints about the default branch name are not shown.*

### Question 2:

```text
$ git status
On branch master
nothing to commit, working tree clean
$ git push origin master
To ../html-remote
 * [new branch]      master -> master
```


### Question 3:

```text
$ git clone html-remote html-copy
Cloning into 'html-copy'...
done.
$ git log --oneline
76568ef Add next meeting heading
e64b025 Add home page
```

The same commits appear in `html-copy` as in `html-lab`.


---

**Result:** All three Git tasks were written to demonstrate creating a remote repository, pushing the commits to it, and cloning it into a new folder.
