# the readme file for Git Exercises

## Bundle 1

### Exercices 1

- Create a project folder & initialize git
```bash
  git init
  ```

- Make changes to the project (add files and contents)
```bash
git add .
 ```

- Rename your main branch from `master` to `main` (If your branch name is already `main` then rename it to `master` and then back to `main`)
```bash

git branch -M <branch>
 ```

- Stage your changes and commit them
```bash
git add . and git commit -m"commit message"
 ```

- Create a Github repo and connect it with your project
```bash
git remote add origin <URL link of your github>
 ```

- Push your changes to GitHub
```bash
  git push origin main
   ```

- Create a new branch `dev`
```bash
  git branch -b dev
   ```
- From `dev` create another branch `test`
```bash
  git branch -b test
   ```
- Go back to the `dev` branch and delete the `test` branch
```bash
  git checkout dev and git branch -d test
   ```

### Exercises 2

- Create a new `home.html` file, add some html changes and save them
- Stash save your current changes
```bash
  git stash
   ```
- Repeat the same process for a new `about.html` page and stash save your changes
```bash
  git stash
   ```
- Repeat the same process for a new `team.html` page and stash save your changes
```bash
  git stash
   ```
- Using stash pop restore the changes of the `about.html` page
```bash
  git stash pop 3
   ```
- With the help of an index use stash pop bring back the `home.html` page changes
```bash
  git stash pop
   ```
- Commit the current changes and push them
```bash
  git commit -m"commit message" and git push origin main
   ```
- Using stash pop restore the changes of the `team.html` page index
```bash
  git stash pop <index>
   ```
- Reset the current changes using git reset and go back to the changes without the `team.html` page
```bash
  git reset --hard
   ```
## Bundle 2

### Exercise 1


- Create a new branch named `ft/team-page`
```bash
git checkout -b ft/team-page
```
- Create a new html page named `team.html` and add some changes

- commit and push those changes

- Create a new PR for the changes
- Go back to `main` branch (checkout the `main` branch)
- Create new branch named `ft/contact-page`
- Go back to the `ft/team-page`
- With the help of git log look for the last commit and copy its hash
- Checkout again `ft/contact-page` using git cherry-pick get the changes from the last commit on the `ft/team-page` branch.
- Add new changes for the contact page and commit, push them
- Create a new PR for the contact page
- From the `ft/contact-page` branch create a new branch called `ft/faq-page`
- Create a new `faq.html` page and add some changes there
- Commit and push those changes
- Using git revert, revert the changes of the last commit of the `ft/team-page` branch. (use the commit hash you copied earlier)
- Push the changes and create a new PR
