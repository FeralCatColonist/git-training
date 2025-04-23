# Directions for Demo 5

Now we're going to wrap up and merge our changes with the main branch. This is the crux of branch-based development. You create a branch to address an issue and then push that into the version that runs in production.

First, let's rename our `hello-world.md` file to start with your first initial and last name like: `jcarmona-hello-world.md`

```bash
git status
```

While we may not realize it, this is going to require two separate actions on our part. First, we'll need to `git add` the deleted file and then `git add` the new name of our file. To us, we abstract away the change of these two objects as a re-naming, but Git doesn't have that perception. To it, those files are separate objects. As a convenience feature, we can utilize:
```bash
git add .
git status
git commit
git push origin <BranchName>
```
The `.` is short-hand for any object that is currently trackable; all of these objects will then be put into staging. This could have some unintended consequences so it is generally better to explicitly add your files by name.
```bash
git commit
git push origin <BranchName>
```
In our commit message let's have the subject line read:

[CGIT-2385] First Name Last Name

And then feel free to fill out the other template fields. Once complete we're ready to merge into the main branch. We'll start by switching to main, then grabbing any new files, then performing a merge against our development branch. The `--no-ff` will preserve branch information so that we're aware of what branch was used to push those commits.
```bash
git switch main
git pull origin main
git merge <BranchName> --no-ff
```