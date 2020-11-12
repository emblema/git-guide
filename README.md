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


## Add a new branch to the local and remote repository

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
