# Source Control Workshop

This workshop is designed to show the basics of how to use Git as your Source Control Management Tool.

## 5 Basic commands you should commit to memory (see what I did there?)
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

### Windows Specific
- Install Putty 
- Generate an SSH Key (if you don't already have one)
    - [Manually generating your SSH key in Windows](https://docs.joyent.com/public-cloud/getting-started/ssh-keys/generating-an-ssh-key-manually/manually-generating-your-ssh-key-in-windows)
		- An SSH key is used to log into your Virtual Machine (You will create one for this lab)

### Mac and Linux Specific
- Generate an SSH Key (if you don't already have one)
    - [Generating a new SSH key and adding it to the ssh-agent](https://help.github.com/en/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

### All Environments
1. A GitHub Account (if you don't already have one)
    - Sign-up for Github [here](https://github.com/join?source=header-home)
		- You can use your MS email address and add a personal one later for recovery and long term purposes
1. An Azure DevOps Account (Create your own new Org!!!)
    - Sign-up for Azure DevOps [here](https://dev.azure.com)
1. A Virtual Machine Running Ubuntu 18.04-LTS Server
    - Ensure that your NSG settings allow/enable port 22 (SSH)
		- Use the public SSH Key (e.g. id_rsa.pub) you generated in the above sections for Windows, Mac/Linux as the SSH Key to log into your server
    - We will be running our workshop on this remote machine to ensure uniformity and to avoid polluting our local environment
		- A "Clinic" session will be run at the end of the workshop to install Git on your local machines (time permitting)
1. [Visual Studio Code Insiders](https://code.visualstudio.com/insiders/)
    - We will be using Visual Studio (VS) Code Insiders to connect and run our workshops in the remote environment using the [Remote Development](https://code.visualstudio.com/docs/remote/remote-overview) feature
		- VS Code and VS Code Insiders also provide other helpful tools to help accelearte our learning (e.g. built in git support, syntax highlighting)

