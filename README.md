# Git Quick Guide (Step by Step)

## Basic Git workflow
### Step 1: Create a new local repository

`mkdir hello-world`

`cd hello-world`

`git init`

### Step 2: Add README file

`echo “# Hello World” > README.md`

### Step 3: Make the initial commit in the local repository

`git status`

`git add .`

`git commit -m “Initial commit”`

### Step 4: Create a new GitHub repository 

Go to this page [New repository](https://github.com/new)

### Step 5: Pushing code to the GitHub repository

`git remote add origin https://github.com/<username>/hello-world.git`

`git branch -M main`

`git push -u origin main`


## Add a new branch
### Step 1: Create a new branch

`git checkout -b new-branch`

### Step 2: Set the upstream branch 

`git push -u origin new-branch`

### Step 3:  Check tracking branches

`git branch -vv`


## Checkout an existing remote branch
### Step 1: Checkout and track the existing branch

`git checkout —-track origin/existing-branch`

### Step 2: Check tracking branches

`git branch -vv`


## Merge changes into the main branch
### Step 1: Switch to main branch

`git checkout main`

`git branch`

### Step 2: Review changes

`git diff main new-branch`

### Step 3: Merge

`git merge new-branch`

`git show`

### Step 4: Update remote

`git push`

`git status`

### Step 5: Delete branch

`git branch -d new-branch`


## Review history
### Step 1: View commit history

`git log --oneline`

### Step 2: View changes in last commit

`git show`

### Step 3: View changes in past commits

`git show HEAD~1`

### Step 4: View a file in a commit

`git show HEAD~1:file.txt`

### Step 5: View all the files and directories in a commit

`git ls-tree HEAD~1`

### Step 6: View a file by its unique identifier

`git show <uid>`
