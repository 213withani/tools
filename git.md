# Merging vs. Rebasing
https://www.atlassian.com/git/tutorials/merging-vs-rebasing

git rebase = git merge: integrate changes from one branch into another branch

new commits in master are relevant to the feature that you’re working on

easy option:
```
git checkout feature
git merge master
```

# Git Blame
https://blog.andrewray.me/a-better-git-blame/

TL;DR git blame rarely gives helpful results. Instead use specific flags on git log to find the true author of a change.

# git checkout -- .

no changes added to commit (use "git add" and/or "git commit -a")
~/Documents/dev/ (701 ✘)✹ ᐅ git checkout -- .
~/Documents/dev/ (701 ✘)✹ ᐅ git status       
On branch 701
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   ../client/src/containers/AccountSpendContainer.js
	modified:   ../client/src/store/index.js

# Need to read
https://itnext.io/become-a-git-pro-in-just-one-blog-a-thorough-guide-to-git-architecture-and-command-line-interface-93fbe9bdb395
