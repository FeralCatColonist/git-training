# Directions for Demo 1

Open the app Git Bash, it has a logo that looks like this. ![it looks like this](https://www.gitkraken.com/wp-content/uploads/2021/07/GitBashLogo.jpg)

Open a browser and navigate to our team's [GitLab repository](https://gitlab.com/some-tenant), then open the project git training. 

In the top right of the project is a clone button, using the drop-down feature copy the URL for the option Clone with HTTPS, it should look like this:
https://gitlab.com/some-tenant/some-project/git-training.git

We are going to do the following two things:
1. Clone the Project into an appropriate folder
2. Create a new branch within the project

With the way the geospatial codebase is structured, the deployment pattern should be that all geospatial projects live within the same umbrella folder. This top-level folder can have any name, and I'd recommend something short. Mine is called `Repository`.

Cloning the project is easy, within git bash, you'll use the following commands, entered one at a time, they are executed with the `enter` button:
```bash
cd "path to your repository"
git clone https://gitlab.com/some-tenant/some-project/git-training.git
```
The above commands changes the working directory (`cd` stands for **change directory**) from whatever is the default to our chosen directory. You can also [change where git bash opens by default.](https://codergrl.com/2019/12/18/change-default-location-for-git-bash-on-windows/)
Now that you are in the umbrella, or root, folder. Then we initiate the `git clone` command, this creates a new folder `git training` and initializes a git architecture-- --which is just a series of hidden files that track stuff that we're definitely not getting into. It is enough to know right now that it exists and that it isn't magic.

Your bash window will have processed some text. What we need to do next is to change into that newly created directory. We again call `cd`:
```bash
cd git-training
```
the bash window will now have the new file path along with the word `(main)` appended to the end. This is how we know what our current branch is. The initial branch of a project within the geospatial repository is called main. The previous common name was used in coding projects by convention was called `master` this was problematic and is no longer the default for new code bases.

Let's also go head and create a branch. There's different opinions. My opinion is that it should be verbose like:
`firstinitiallastname/jira-issue/add-demo-1-contents`
The code to do it is pretty easy:
```bash
git checkout -b jcarmona/ESRI-470/name-what-your-branch-does
```

You'll notice that the (main) has now changed to reflect your chosen branch name (whatever-your-branch-name-is)

And just a quick final note here. Spaces matter and cannot be used as paths, so if we have paths with spaces they need to be wrapped in `""`. Git branches cannot contain spaces.

Lastly, if we wanted to switch between branches, we do that with `git switch`:
```bash
git switch main
git switch jcarmona/ESRI-470/add-demo-1-contents
```