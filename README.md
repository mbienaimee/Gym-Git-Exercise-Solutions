# the readme file for Git Exercises

## Bundle 1

### Exercices 1

- Create a project folder & initialize git
  git init

- Make changes to the project (add files and contents)

git add .

- Rename your main branch from `master` to `main` (If your branch name is already `main` then rename it to `master` and then back to `main`)

git branch -M <branch>

- Stage your changes and commit them

git add . and git commit -m"commit message"

- Create a Github repo and connect it with your project

git remote add origin <URL link of your github>

- Push your changes to GitHub

  git push origin main

- Create a new branch `dev`
  git branch -b dev
- From `dev` create another branch `test`
  git branch -b test
- Go back to the `dev` branch and delete the `test` branch
  git checkout dev and git branch -d test

### Exercises 2

- Create a new `home.html` file, add some html changes and save them
- Stash save your current changes
  git stash
- Repeat the same process for a new `about.html` page and stash save your changes
  git stash
- Repeat the same process for a new `team.html` page and stash save your changes
  git stash
- Using stash pop restore the changes of the `about.html` page
  git stash pop 3
- With the help of an index use stash pop bring back the `home.html` page changes
  git stash pop
- Commit the current changes and push them
  git commit -m"commit message" and git push origin main
- Using stash pop restore the changes of the `team.html` page index
  git stash pop <index>
- Reset the current changes using git reset and go back to the changes without the `team.html` page
  git reset --hard

## Bundle 2

### Exercises 1

- Create a new branch named `ft/bundle-2`
  git branch -b ft/bundle-2
- Add new changes to your project. create a new page named `services.html` and add some changes
- Commit your changes and create a Pull Request against the `main` branch in your github repository
   git push origin ft/bundle-2
- Request a review and make sure your Pull request gets merged (Look for someone to merge your PR)
   git pull origin main

### Exercise 2

- Checkout your `main` branch and pull the latest changes
  git checkout main and git pull origin main
- Create a new branch named `ft/service-redesign`
  git branch -b ft/service-redesign
- Add new changes to the `service.html` page
  git add service.html
- commit and push them
  git commit -m"commit service.html" and git push origin ft/service-redesign
- create a new PR for your changes
  Raise pull request
- go back to your `main` branch and add again new changes to your `service.html` page, you can add different changes but make sure to affect the same part(line of code) as you did in the other PR
- Commit and push those changes
- Now go back to the Github PR you had created for the `ft/service-redesign`branch, you will then see that you have conflicts with the `main` branch
- In your project checkout the `ft/service-redesign`branch
- Compare the `ft/service-redesign`with the `main` branch using git diff and observe the changes
- Using git merge, merge the `main` branch with `ft/service-redesign` branch and commit and push you changes again