# Modifying, Adding, Committing and Pushing Changes

The whole point to source control is to create and contribute changes to a project.  Here we'll make some trivial changes to our project and commit them to histroy.

## Modifying
Let's make a change to this file.

```<Replace me with your name>```

Now let's ```commit``` our change by running the following commands:

- ```git add -u```
- ```git commit -m "adding my name to this project"```
- ```git push```

Congrats! You've just modified a file.  In reality you'd be adding more than just your name but the idea is still the same.  Things will get complicated however when you're working on the same file as a peer. This is when we need to think about roles such as a "Code Master" or lead developer/engineer who will handle these "Merge Conflicts" but that's a lesson/pain for another day :D

## Adding new files
Let's add a new file to this project.

In the current directory (```source_control_workshop/labs```), let's add a new file called ```your_full_name.md```.  In this file, just write some arbitrary text...mash your keyboard.  Let's save the file.

Now let's ```add``` our file to the project by running the following commands: 

- ```git add -A``` or ```git add .```
- ```git commit -m "iterating and innovating like a pro"```
- ```git push```

You're done! You've now added a new file to your project.  View this and the modified change(S) you've made on Github!