# Source Control Workshop

This workshop is designed to show the basics of how to use Git as your Source Control Management Tool. THis is an example of an update.

## 4 Basic commands you should commit to memory (see what I did there?)
- ```git pull```
- ```git add -A```
- ```git commit -m "some commit message"```
- ```git push```
	- Push commited file changes to current branch
	- use the ```-u upstream_server/branch_name``` to push/save to a different server/branch

## Advanced commands you should be aware of
- See what branch you're currently working on
	- ```git branch```
- Checkout and create a new branch
	- ```git checkout -b <branch_name>```
- Merge changes from your branch into another one (3 steps)
	- Ensure your changes are added/tracked (```git add -A```) 
	- Ensure your changes have been committed to your current branch
	- Checkout your target branch (the branch you want to merge into)
		- ```git checkout <branch_name>```
	- Merge Changes from your Source/Feature Branch and fix any conflicts
		- ```git merge <source_branch_name>```

## Requirements

These are the minimum requirements to run this lab.

### All Environments
1. A GitHub Account (if you don't already have one)
    - Sign-up for Github [here](https://github.com/join?source=header-home)
		- You can use your MS email address and add a personal one later for recovery and long term purposes
1. [Visual Studio Code Insiders](https://code.visualstudio.com/insiders/)
    - VS Code and VS Code Insiders also provide other helpful tools to help accelearte our learning (e.g. built in git support, syntax highlighting)
1. Git Installed on your Machine:
	- [Windows](https://github.com/git-for-windows/git/releases/download/v2.22.0.windows.1/Git-2.22.0-32-bit.exe)
	- [Mac](https://sourceforge.net/projects/git-osx-installer/files/git-2.21.0-intel-universal-mavericks.dmg/download?use_mirror=autoselect)
	- Linux:
		- Debian systems: ```sudo apt-get install git```
		- RedHat systems: ```sudo yum install git-core```

### Alternative Path
You can also run this lab (minus installing Git) in an Azure Cloud Shell (https://shell.azure.com).  Git is already installed and you can run a version of VS Code in the browser along side your terminal as well.