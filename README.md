# My git Memento

`To begin with`
- git init: create a git repository in current directory (you should only do this once in a repository, i.e. no nested git repositories)

`Most useful commands`
- git status: tells you what is going on
- git add `<filename>`: put a file in the staging area
- git restore --staged `<filename>: to unstage a file
- git commit: commit the file to the branch master
	- git commit -m "`<message>`": commit with a message without opening up text editor

`Explore history`
- git log: journal with all commit messages
	- git log --oneline: simplified view of the log. Note in particular the HASH for each commit (i.e. number identifying a commit)
- git diff `<filename>`: looks at differences between HEAD (i.e current state) and previous commits
	- git diff HEAD~2 `<filename>`: looks at differences between current state (HEAD) and the last 2 commits 
	- git diff `<HASH>` `<filename>`: looks at differences between current state (HEAD) and the commit identified by the HASH number.

`Revert changes`
NB: Dont't forget to add and commit afterwards if you want to save the restored version.			
- git checkout `<HASH>` `<filename>`: moves back to the status in the commit whose number is HASH
- git restore `<filename>`:restore file before changes for an unstaged file

`Ignoring files`
* Create a .gitignore file with Sublime in the current directory.
	subl .gitignore
* Write in the .gitignore file the names of all the files you don't want to follow (whole filenames or regular expressions).
* Stage (add) and push (commit) the  .gitignore file on the master branch.

`Conflicts`
When there are two different versions on your machine and GitHub and the git pull origin master won't work (conflicts between versions)
* Solve conflicts with a GUI.
* Redo a commit on your local machine.
* Redo a push.