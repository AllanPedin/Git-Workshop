# Git-Workshop
This is a workshop intended to help people understand git with respect to working on a project with multiple collaborators
# Cloning a repo
```
git clone <repo uri>
```
# Make some changes
```
console.log("Hello <Your name>!")
```
# Stage your changes
```
git add .
```
# Commit your changes
```
git commit -m "Added Hello World"
```
Commit is like making a save file, youll always be able to go back and look at your old commits
# Push your commit
```
git push
```
Push takes your local commits and pushes them to a remote repository. Just like uploading something to the cloud
### Pushing may fail
If you try to push and code gets rejected due to (non-fast-forward) that means someone else has pushed their commits before you did. In order to fix this you must retrieve their code from the remote repository and merge it with your code.
# Pulling others commits
```
git pull
```
# Solving merge conflicts
If two developers have made changes to the same file, who ever pushes their changes last gets to decide the final state of the code.

Current changes -> the changes you commited

Incoming Changes -> the changes someone else commited

![Solving merge conflicts in vscode image](https://github.com/AllanPedin/Git-Workshop/blob/main/solving_merge_conflicts.png)

To solve the merge conflicts you can use VScode. You can either accept your changes, the changes someone else commited, or a combination.

Once your done resolving the merge conflicts you can:

```
git add .
git commit -m "solving merge conflicts"
git push
```
# Separateing your code into different files with different purposes can help to reduce the amount of merge conflicts
Make a new file and name it your first name, then send it up to the remote repository:
```
git add .
git commit -m "added my new file!"
git push
```
# Branches
Branches are a tool to help projects with multiple developers work together without as many conflicts

Show available branches:
```
git branch
```

Checkout my branch
```
git checkout AllansFeatureBranch
```

Go back to the main branch
```
git checkout main
```

Make your own branch
```
git checkout -b <your branch name>
```
make some changes and push it to the remote repository
```
git add .
git commit -m "made some changes on my new branch"
git push
```
