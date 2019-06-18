# Branching

Branching allows us another mechanism to make changes without polutting or interfering with our project and peers/collaborators.  Branching is associated with our current working repository and thus will not interfere with the original repository we have forked from.

Generally we will make our changes in our own branches ("feature" branches), merge them back to our master branch (this could also be a development or "release" branch...will explain this later) and then submit a pull request back to the original project (optional - only if you intend to contribute back to the orignal project).

You will often encounter questions from developers around branching strategies.  Please see [09_branching_and_flow_strategies](09_branching_and_flow_strategies.md) for more details.

## Creating a branch!
Let's create our own branch!

Let's run the following commands:

- ```git checkout -b <your_name>``` REPLACE ```<your_name>``` with...your name (e.g. ```raykao```)
	- This will create a new branch with the name specified
	- Usually this is related to a feature, bug/hot fix, issue etc.

That's it, you've now created a new branch of your code to work in. Your original (```master```) branch lives in a different parallel branch and for all intents for now, lives in it's own snapshop in time.  You can switch back to that branch by using the ```git checkout master``` command to return to the master branch.  **Note:** that any changes you made in the ```<your_name>``` branch will not appear in ```master``` branch until you run a ```git merge```.  More on this in a later lab ([04_merging_changes.md](04_merging_changes.md)).

Next let's start contributing to our project.

## Further Reading
- [Don’t Mess with the Master: Working with Branches in Git and GitHub](https://thenewstack.io/dont-mess-with-the-master-working-with-branches-in-git-and-github/)