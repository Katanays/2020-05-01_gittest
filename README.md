#Memento git

`To begin with`
`
`Most useful commands`
- git status: tells you what is going on
- git add `<filename>`: put a file in the staging area
- git restore --staged `<filename>: to unstage a file
- git commit: commit the file to the branch master
	- git commit -m "<message>": commit with a message without opening up text editor

`Explore history`
- git log: journal with all commit messages
	- git log --oneline: simplified view of the log (note in particular commit numbers)
- git diff <filename> :looks at differences between current state and previous commits
	-git diff HEAD~2 <filename>: looks at differences between current state (HEAD) and the last 2 commits 
	-git diff <commit_number> <filename>: looks at differences between current state (HEAD) and the given commit

`Revert changes`
NB: Dont't forget to add and commit afterwards if you want to save the restored version.			
- git checkout <commit_number> <filename>: moves back to the status in the given commit 
- git restore <filename>:restore file before changes for an unstaged file

`Ignoring files`
* Create a .gitignore file with Sublime in the current directory.
	subl .gitignore
* Write in the .gitignore file the names of all the files you don't want to follow (whole filenames or regular expressions).
* Stage (add) and push (commit) the  .gitignore file on the master branch.

