# Git:
Version control system(track changes in code), free, open source, fast, scalable

# GitHub:
allows developers to store & manage their code using Git.

# Commands:
1.Cloning existing repo=
	• git clone <-HTTP link->
	• git status
		○ untracked
		○ modified
		○ staged
		○ unmodified
	• git add <-file name->(save all changes, status should be ready to commit)
	• git add .(ad all)
	• git commit -m "some msg"
	• git push origin main(will push to the repo on GitHub)

2.New repo=
	• git init(making repo a git repo)
	• git remote add origin <-link->(add the link we get after creating a new repo w/o readme)
	• git remote -v(to verify remote)
	• git branch
	• git branch -M main(to rename branch)
	• git push(-u) origin main(-u then don't have to write origin main again)

3.Branch commands=
	• git checkout <-branch name->(to navigate)
	• git checkout -b <-new branch name->(to create branch)
	• git checkout -d <-branch name->(to delete)

# Merging code:
1.Way 1- through command line
	• git diff <-branch name->(to compare commits, branches, files & more)
	• git merge <-branch name->(to merge 2 branches)

2.Create a PR(pull request) on GitHub
	• Have to generate a PR on GitHub & merge it there only
	• git pull origin main(for changes in local storage) 

# Resolving merge conflicts:
If change in same part in different branches and we are trying to git merge then vs code will give some options

# UNDO changes:
1.Staged changes(changes which are added but not commited)
	• git reset <-file name->

2.Commited changes
	• git reset HEAD~1(for one commit)
	• for many commits
		○ git reset <-commit hash->
		○ git reset --hard <-commit hash->


* git log (for checking commits)


# Fork:
It is a rough copy.
Fork is a new repo that shares code and visibility settings with the original "upstream" repository.
