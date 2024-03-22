Create and move to a new orphan branch. This branch will be used as a replacement for the main branch later.
Orphan branch is a branch with no parent commit history
```bash
git checkout --orphan new-branch
```
You need to add all files in our project to the git again.
```bash
git add -A
```
Commit your files. This will be your initial commit history in the current branch.
```bash
git commit -m "commit message"
```
Delete the old gh-pages branch.
```bash
git branch -D gh-pages
```
Rename the current branch to gh-pages.
```bash
git branch -m gh-pages
```
force update to the gh-pages branch in your remote repository.
```bash
git push -f origin gh-pages
```
