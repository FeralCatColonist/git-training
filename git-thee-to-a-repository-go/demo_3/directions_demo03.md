# Directions for Demo 3

We're doing a few things here. Mostly house-keeping, a little git.

I'm assuming you're using VSCode because it is the best. Let's go ahead and download the GitLens Extension, you'll click  the extensions widget on the left side of the VSCode screen. At the top of the you can type in: `GitLens`

The first result should be GitLens -- Git superchaged by GitKraken; left click and install it.

We're not going to talk about it, but you might as well download the following, all from Microsoft:
- Black Formatter
- Flake8
- isort
- Jupyter
- Jupyter Cell Tags
- Jupyter Keymap
- Jupyter Notebook Renderers
- Pylance
- Python

We are going to set up a commit template. I looked far and wide and [chose this one](https://github.com/joelparkerhenderson/git-commit-template). With Bash open and in the root folder we'll run the following code:
```bash
git config commit.template .gitmessage
```
And you could of course set a global commit template; you'd make a copy of the `.gitmessage` and put that in the root of your user directory on your computer. A locally configured git commit template will take precedence over a global config template. You'd set it like this:
```bash
git config --global commit.template ~/.gitmessage
```

So hopefully now we'll get a little bit of clarity. We're ready to make our first commit and push.
```bash
git commit
```

This will open the template that we just configured within our IDE. Everything in green is commented out and will not be visible within the final message. Commit messages are not required by default-- --and that's totally not helpful. So a template helps us enforce standards for ourselves and for others. Before we do anything here, let's go around and check out what some of these messages look like fully formatted:

- `Scrubbed`
- `Scrubbed`
- `Scrubbed`

So now that we've seen the variations for what that commit message could look like, let's go ahead and fill out the commit message for our `Hello World!` file. A few notes before we proceed, line spacing matters, so if there's a line break in the template preserve it in your final copy.
- Subject line would be something like, `[ESRI-2385] Add Hello World File`
- Why, because we're doing a demo.
- How can just describe the method you used to build that file.
- Tags can be set to `demo,`

Finally, our files have been commited into our branch. This means that there is a new version snapshot. We can view this behavior by through `git log` and you can escape the `git log` by entering `q`. Your git has two distinct versions, or commits; the first was at the time of the branch creation, and the second just now when we used the `git commit` command. At this moment it only lives on your local machine, we're going to change that now:
```bash
git push -u origin <name-of-your-branch>
```
the verbose form of this command looks like this:
```bash
git push --set-upstream <remote-name> <name-of-your-branch>
```
we can double check the name of our remote, by convention it is called `origin` through the following command:
```bash
git remote -v
```