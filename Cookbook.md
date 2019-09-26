**Checkout a Remote Repository**

	git clone urltoRepo.git


**Add Files To Git Ignore**

	Add file names to .git/info/exclude for the files you want to be ignored when adding to files to commit

**Commit Files To Remote Repo**

	First stage the desired files with:

**git add path to files**

	After that commit the files to the local repo with 

    git commit -m “Commit message”

**Add a remote repo if not done before**

	git remote add origin andre_marcos@bitbucket.org/andre_marcos/life_stats.git


**Stage Files Deleted Manually**

	git rm $(git ls-files --deleted)


**Push Branch to Remote Repo**

	git push --set-upstream origin feature-PROD_VSB-524


**Revert Uncommited changes of File**
	
	git checkout file_name


**Create and Switch to Branch**

	git checkout name_of_branch
	

**Delete Branch**

	git branch -d name_of_branch

**Diff staged Files**

	git diff --staged

**Unstage all Files**

	git rm --cached -r .

**Unstage a File**

	git reset HEAD file_path

**Uncommit last commit**

	git reset --soft HEAD^

**git Checkout remote branch**

	git branch feature/PROD_VSB-222 origin/feature/PROD_VSB-222
	git checkout  feature/PROD_VSB-222


**git merge two branches**

	git checkout feature/PROD_VSB-222
	git merge develop

	--merges develop into feature/PROD_VSB-222

**Get Remote Repository URL**

	git config --get remote.origin.url


**Remove A Directory From Repo without removing it Locally**

    git rm --cached -r .settings/


**Configuer User**

    git config --global user.name "John Doe" 
    git config --global user.email johndoe@example.com


**Diff between local repo and remote repo (diff of what is still not pushed but has been commited)**

	git diff origin/master..HEAD
