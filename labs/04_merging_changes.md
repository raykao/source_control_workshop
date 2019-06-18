# Merging Changes

Creating code in an isolated branch is not very useful in practice.  You may want a different branch for different target environments (test, dev, staging, pre-prod, prod... etc.).

Eventually you'll want to promote your code to the master branch (this may also be called the release branch...).  Most Companies/Teams use the master branch as the main source of truth for code.  Meaning that all other branches will stem from this main trunk.  All independent changes will be contributed back into the master branch and all future development and updates will be branched off of master.  This is how we ensure we take advantage of each other's hard work in an organized manner and without overwritting each other's work.  

**Note:** There's usually a handful of "Code Masters" who are repsonsible for approving changes and handling any conflicts in code.

## Merge

Let's merge our branched code.

- Let's check which branch we're on:sadfasdfds
	- ```git branch``` you should see your branch name highlighted (e.g. ```<your_name>```)
- Let's now checkout our master branch
	- We need to switch over to the branch we wish to merge INTO
	- ```git checkout master```
- Let's now merge our branched code INTO master
	- ```git merge <your_name>``` -> **REMEMBER** we've been working and making changes in our own independent branch
- Assuming there's no conflicts...your changes have been merged with the master branch
- Let's push the changes up to GitHub
	- ```git push```
	- This now pushes the current local master branch up to our remote master branch on GitHub
		- This makes our changes available to other team members
		- Gives us a centralized way to track the changes
		- If your laptop ever gets destroyed, you can always clone/download a copy of your work
- That's it! You've now merged your changes form your branch into master and have made it available to everyone else on GitHub! Congrats!

Let's now try to submit all these changes into the ORIGINAL project...let's try our first pull request!