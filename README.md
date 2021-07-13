# Git-Workshop

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
## Pushing may fail
If you try to push and code gets rejected due to (non-fast-forward) that means someone else has pushed their commits before you did. In order to fix this you must retrieve their code from the remote repository and merge it with your code.
# Pulling others commits
```
git pull
```
