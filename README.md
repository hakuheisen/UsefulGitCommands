# UsefulGitCommands
GIT STASH
---------
git stash    (save the status of your objects but this is NOT a commit)
git stash list  (list all your stashes of the branch)
git stash apply  (apply the latest stash again on your current branch)
git stash apply stash@{2}   (apply a previous stash (not the latest) on your current branch)
git stash drop  statsh@{2} (remove the indicated stash without reapplying)
git stash show -p statsh@{2} | git apply -R  (unapply the indicated stash or said otherwise reverse apply the indicated stash)
git stash branch (create a new branch from your stash without applying it to the current branch)

CLONE
------
existing repo:  git clone //user@domain.com/repo.git
local repo creation:  git init

LOCAL CHANGES
-------------
git status (show changed files in your working dir)
git diff (changes to tracked files)
git add . (add current changes to next commit)
git add -p <file> (add changes in <file> to next commit)
git commit -a (commit all local changes in tracked files)
git commit (commit previously staged changes)

COMMIT HISTORY
--------------
git log (show all commits, starting with the newest)
git log -p <file> (show changes over time for a specific file)
git blame <file> (who changed what and when in <file>)

BRANCHES and TAGS
-------------------
git branch (list all existing branches)
git branch -v (see last change on a branch)
git branch --merge (list of all branches merged into current branch)
git branch --no-merge (list of all branches NOT merged into current branch)
git checkout <branch> (switch to branch)
git branch <new branch> (create a new branch based on a remote branch)
git checkout -b feature develop (create a new feature branch called feature from branch develop and also switch to it)
git branch --track <new branch> <remote branch> (create new tracked branch based on a remote branch)
git branch -d <branch> (delete a local branch)
git tag <tag name> (mark a current commit with a tag)
git remote update --prune      (refreshing the list and the info on remote branches you have locally)
git branch -m old_branch new_branch  (rename a branch)
git branch -a (show all branches in the list: local as well as remote)
