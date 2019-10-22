# git
Git Related CMD and More Notes on it

### Basic Git CMD
-----
`git init`

`git add README.md`

`git commit -m "<commit_message>"`

`git remote add origin <URL>`

`git push -u origin master`

`git rm -r --cached .`

`git add .`

`git commit -m "<Commit>"`

`git push -u origin master`

`rm -rf .git`

`git init`

`git add .`

`git commit -m "Initial Commit"`

`git remote add origin <URL>`

`git push -u --force origin master`

## STASH
`git stash`

`git stash list`

`git stash apply`

`git stash apply <stash number>`

`git stash push -m "<commit_message>"`

`git stash drop <stash number>`

`git stash pop <stash number>`

`git stash clear`


## Get list of file changes in a commit
`git show --pretty="" --name-only <commit_hash>`

`git diff-tree --no-commit-id --name-only -r <commit_hash>`

`git ls-tree --name-only -r <commit_hash>`


## Know that local branch head is forward of backward
`git fetch origin`

`git status`

## Pull a branch to local repository:
`git pull origin <branch name>`

## Push a branch to the remote repository:
`git push -u origin feature_branch_name`


## Remove/Untrack a file from git
`git rm --cached <file>`

## Merge Multiple Commits
`git rebase -i HEAD~[N]	 #remove the brackets`

`git push -u origin new-branch --force`

## Proxy Configuration
`git config http.proxy http://192.168.49.1:8282`

`git config --get http.proxy`

`git config --global --unset http.proxy`

`git config --system --get http.proxy`

`git config --global --get http.proxy`

`git config --system --get https.proxy`

`git config --global --get https.proxy`

## Making release or tags
`git tag`

`git tag <tag_name>`

`git tag v1.0`

## Anotated tag
`git tag -a v1.1 -m "<message>"`

`git push origin <tag_name>`

## Push all tags at once
`git push origin --tags`

`git push --tags`

`git checkout -b <give_branch_name> <tag_name>`
