# Directions for Demo 4

Now we're going to create a conflict. Or rather, we're going to experience a conflict.

First, let's pretend like we were in the middle of some work, we'll have it staged and we aren't quite ready to commit it to our branch. At the same time, there an update that we'd like to pull from a certain branch. This would be an opportunity for us to use `git stash`. Let's walk through it!

```bash
echo "Some work we are doing" > some-new-file.txt
git add some-new-file.txt
git pull origin conflict-with-stash
```

We'll receive a message from the console that has some stuff like:
```bash
error: Your local changes to the following files would be overwritten by merge:
  git-thee-to-a-repository-go/some-new-file.txt
Merge with strategy ort failed.
```
We are able to protect our work by stashing it away; while we are only working with one file, this command takes a snapshot of your entire working directory.
```bash
git stash
git pull origin conflict-with-stash
```
Now the `git pull` is successful and we can restore our staged changes:
```bash
git stash pop
```
And let's say that maybe, we didn't want that `some-new-file.txt` at all. We can run:
```bash
git reset --hard
```
Which will overwrite your working directory to that state it was in at the time of your last commit. Now we're ready to take a quick look at a merge conflict.
```bash
git pull origin conflict-with-merge
```
You'll receive an error message that ends with `Automatic merge failed; fix conflicts and then commit the result.` You'll also notice that the Bash prompt will change from your `(BranchName)` to `(BranchName|MERGING)`. This is because Git it now in the process of trying to merge these two separate commit instances. If you want to crawfish your way out of this, you can use this to cancel:
```bash
git merge --abort
git status
```
This unwinds the merge and lets us go back to what we were doing. If you get a merge conflict like this, it is best to let someone (probably me) know about it and we can figure out how we want to work through the conflict. Now, let's walk through fixing a merge in-line would look like:
```bash
git pull origin conflict-with-merge
```
We'll open up our IDE and take a look at it. While we're doing this as a file-to-file thing; conceptually, this will happen any time you overwrite a line that has been written by someone else, if the main has been updated since the creation of a feature branch. [This video](https://www.youtube.com/watch?v=HosPml1qkrg) was really helpful in explaining merge conflicts.

For the purposes of our demo, we'll replace the first line with what we wrote and make sure to add the second line from the `conflict-merge` branch because it is funny.