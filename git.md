git config core.editor notepad

branch to master:
	git checkout master
	git pull origin master
	git merge test
	git push origin master
	
delete local branch:
	git branch -d branch_name
	
delete remote branch:
	git push origin --delete <branch_name>