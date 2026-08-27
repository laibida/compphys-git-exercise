# Instructions
## Clone this git repository to your laptop:

```
git clone git@github.com:ubsuny/compphys-git-exercise
```

## Exercise 1: a simple git add/commit/push
1. Copy the file `template.md` to `<your github username>.md` (just work in your local `main` branch, don't worry about creating a new branch).
2. Open the new file in a text editor and answer the questions.
3. Commit the new file to your local git repo. Specifically:
    1. Stage the file (i.e., tell git you want this file in your next commit) with `git add <your github username>.md`
    2. Do `git status` to see what happened.
    3. Commit the file (wrap up the staged files into a commit) with `git commit -m "type a log message"`)
    4. Do `git status` again to see what happened.
    5. Do `git log` to see your commit, now permanently recorded in the history of this branch.
4. Push the files to the remote repo on github.
   1. `git push` (or `git push origin main` to be more explicit)
5. Check that you can see the updates on github.com (i.e. open a web browser and find the updated files). 

If you can see the updates on github, then the instructor can see them, too. When we get to homework assignments, this counts as "turning in" the assignment. You can continue pushing more changes until the due date (or beyond, depending on the instructor). 

## Exercise 2: creating a new branch
1. Inside your local `compphys-git-exercise` folder, create a new branch. Choose a unique name, for example including your github username, so it doesn't conflict with other students.

```
git switch -c <your github username>-test
```

`git switch` is the overall command for switching between branches. The `-c` flag **c**reates a new branch, so this command basically creates a new branch, and then switches to it. 

2. Make a modification to `<your github username>.md`. For example, add your favorite color at the bottom.
3. Repeat the git add/commit/push, except instead of pushing to the `main` branch on github, let's push to a new branch on github:
```
git add <your github username>.md
git commit -m "Test commit for new branch"
git push origin <new branch name>
```
4. Head over to github and find your new branch, now on the remote GitHub repo.
5. Bonus: create a pull request (there should be a big green button). Pull requests are a GitHub-specific feature (not part of git), but are a key part of managing software projects.

