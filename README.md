#Memento git
- git init: create a git repository in current directory (you should only do this once in a repository, i.e. no nested git repositories)
- git status: tells you what is going on
- git add <filename>: put a file in the staging area
- git restore --staged <filename>: to unstage a file
- git commit: push the file on the branch master
	- git commit -m "<message>": commit with a message without opening up text editor
- git log: journal with all commit messages
	- git log --oneline: simplified view of the log
- git diff <filename>:looks at differences between current state and previous commits
		-git diff HEAD~2 <filename>: looks at differences between current state (HEAD) and the last 2 commits 
		-git diff <commit_number> <filename>: looks at differences between current state (HEAD) and the given commit

blabla
blabla
blabla
