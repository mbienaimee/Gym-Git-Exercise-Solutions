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

 # Bundle 2

## Exercises 1

- Create a new branch named `ft/bundle-2`
```bash
git checkout -b ft/bundle-2
```
- Add new changes to your project. create a new page named `services.html` and add some changes
```bash
 git add .
 ```
- Commit your changes and create a Pull Request against the `main` branch in your github repository
```bash
git commit -m"commit message"

```
- Request a review and make sure your Pull request gets merged (Look for someone to merge your PR)
  - created  and Raised new PR

  ### Exercise 2

- Checkout your `main` branch and pull the latest changes
```bash
git checkout main

```
- Create a new branch named `ft/service-redesign`
```bash
git checkout -b ft/service-redesign
```
- Add new changes to the `service.html` page
  - add changes to the file which called service.html
- commit and push them
```bash
git add .
git commit -m"commit message"
git push
```
- create a new PR for your changes
   - Create new PR and raise it
- go back to your `main` branch and add again new changes to your `service.html` page, you can add different changes but make sure to affect the same part(line of code) as you did in the other PR
```bash
 git checkout main
 ``` 
   - Add new changes in service.html
- Commit and push those changes
```bash
git add .
git commit -m"commit message"
git push
```

- In your project checkout the `ft/service-redesign`branch
```bash
ft/service-redesign
```

- Compare the `ft/service-redesign`with the `main` branch using git diff and observe the changes

  - Then I compared  the branches to see the changes
- Using git merge, merge the `main` branch with `ft/service-redesign` branch and commit and push you changes again
 ```bash
  git merge
  git add .
  git commit -m"commit message"
  git push 
  ```
## Bundle 3

### Exercise 1


- Create a new branch named `ft/team-page`
```bash
git checkout -b ft/team-page
```
- Create a new html page named `team.html` and add some changes

  - I created team.html file and make some changes in it

- commit and push those changes
 ```bash
  
  git add .
  git commit -m"commit message"
  git push origin ft/team.html

  ```


- Create a new PR for the changes

   - After pushing I created and raised PR

- Go back to `main` branch (checkout the `main` branch)
```bash
 git checkout main

 ```
- Create new branch named `ft/contact-page`
```bash
 git checkout -b ft/contact-page
 ```
- Go back to the `ft/team-page`
```bash
git checkout ft/team-page
```
- With the help of git log look for the last commit and copy its hash
```bash
 git log

 ```
- Checkout again `ft/contact-page` using git cherry-pick get the changes from the last commit on the `ft/team-page` branch.
```bash
 git checkout ft/contact-page
 git cherry-pick hash
 ```
- Add new changes for the contact page and commit, push them
```bash
git add .
git commit -m"commit message"
git push

```

- Create a new PR for the contact page

  - creating and raising New PR
- From the `ft/contact-page` branch create a new branch called `ft/faq-page`

```bash
 git checkout -b ft/faq-page

 ``` 

- Create a new `faq.html` page and add some changes there

  - create faq.html
- Commit and push those changes
```bash
git commit -m"commit message"
```
- Using git revert, revert the changes of the last commit of the `ft/team-page` branch. (use the commit hash you copied earlier)
```bash 
git revert
```
- Push the changes and create a new PR
```bash
git add .
git commit -m"commit message"
git push

```

## Exercise 2:

- Create new branch from the `ft/faq-page` branch named `ft/home-page-redesign`
```bash
 git checkout -b ft/home-page-redesign

 ```
  
- Go back to the `main` branch and make some changes there
```bash
 git checkout main
```
  - And perform some changes

- Commit and push them
```bash
git add .
git commit -m"commit message"
git push
```
- go back to the `ft/home-page-redesign` branch
```bash
git checkout ft/home-page-redesign

```
- Using git rebase, rebase your branch to `main`
```bash
git rebase
```
- Add changes to the home page and commit push them
```bash
git add .
git commit -m"commit message"
git push
```
- Create a PR for the changes.
  - I created and raised a new PR

# Bundle 4

## Exercise 1

- Checkout the `main` branch
```bash
 git checkout main
 ```
- Create a new repository on Github
  - created new repository  
- Using git remote add the repo to your project as second remote named `git-copy`
```bash
git remote add git-copy link

```
- Make a new changes on the home page

  -make changes on home page

- Commit the changes
```bash
git commit -m"commit message"
```
- Push the changes to the both remotes. the `origin` and `git-copy`
```bash
  git push origin
  git push git-copy

  ```

## Exercise 2

- Checkout a new branch named `ft/footer`
```bash
git checkout -b ft/footer

```
- Add some changes to the branch and commit them
```bash
git add .
git commmit -m"commit message"
```

- Add more changes again to the branch and create a second commit

```bash
git add .
git commit -m"second commit"

```
- Push and create a new PR for the branch
```bash
git push
```
- Checkout the `main` branch again
```bash
git checkout main
```
- From there create a new branch named `ft/squashing`
```bash
git checkout ft/squashing
```

- Using git merge squash, squash the changes on the `ft/footer` branch
 ```bash
 git merge ft/footer
 ```
- Commit the changes with a different commit message such as `footer changes squashing`
```bash
git commit m"footer changes squashing"

```
- Push the changes and create a PR
```bash
git push
```
 - after I created and raise PR
