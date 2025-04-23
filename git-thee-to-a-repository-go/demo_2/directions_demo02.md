# Directions for Demo 2

The Git Bash app should be opened still. If not, follow the directions in the [demo 1 readme.](..\demo_1\directions_demo01.md) To recap, your Git Bash should be:
- opened to the project folder
- in a new named branch

The next command we'll look at is the `git pull`, this grabs any new files from the origin or source project. In our instance GitLab. So let's do that:
```bash
git pull
``` 
We should get an error like the following:
```text
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> jcarmona/ESRI-470/add-demo-2-contents
```

The reason for this is that our new branches are not registered with GitLab just yet. They only exist locally on our machines. This is the crux of the pull. We sync our project against a source. Normally, we do this to keep our files up-to-date between our computer (the remote) and our gitlab repository (the origin) but we can also use the git pull to sync between multiple remotes or to grab specific items from other branches. Again, probably beyond the scope of our codebase but it it nice to be aware of the concepts.

So let's go ahead and do the thing that we always do when we learn new computer stuff. A Hello World. You can use your file system to create a `.txt` file, create within your IDE, or we can do it from Bash. Let's Bash it.
```bash
cd git-thee-to-a-repository-go/demo_2
touch hello-world.md
```
Now let's open that file and add the text: `Hello World!`
Then let's push that file into the staging area with the following command:
```bash
git add hello-world.md
```

Finally we're in a place to see something interesting. Let's utilize `git status` to see what changes we have pending within our repository :
```bash
git status
```
You'll see that have a single file that is staged for commit. We'll leave it here for now!