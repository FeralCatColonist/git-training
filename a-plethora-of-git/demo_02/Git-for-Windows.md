#### [return to demo-02](directions-demo-02.md)
# Directions for Git for Windows

Open Git Bash. We will eventually enter the following commands:

```bash
cd "the-path-to-your-directory/git-training"
git switch -c the-name-of-your-new-branch
```

This:

- changes the directory (folder) the bash terminal is pointed to
- `git switch`<sup>1</sup> with the `-c` flag (short for --create) does the following:
  - creates a new `branch` with the `-c` flag
  - `checkout` the new `branch`

> While we do not have standards at this point, our advice is to make the name descriptive in what
> you are trying to accomplish. A few examples:
> 
> - `build-locator-parcels`
> - `upgrade-geodatabase-automation`
> - `refactor-getpalsinfo-gp-tool`
> 
> The idea here is that if anyone stumbles upon your `branch` it should be clear as to its purpose.
> Also, the `branch` name is recorded in the logs and will appear when you `merge` your changes into
> main. 
> 
> A few notes, you:
> 
> - can use capital letters but those get forced down to lowercase
> - should prefer `-` over `_` since a `-` is both more legible and easier to type than a `_`
> - cannot use names longer than 62 characters, they are truncated (in bitbucket)
> 
> Fill out the `branch` name, since this is a training demo, you can use a pattern like:
> 
> - `jcarmona-git-demo`

Now we can enter the bash command in our Git Bash terminal:

```bash
cd "the-path-to-your-directory/git-training"
git switch -c jcarmona-git-demo
```

**You've now created a new branch in the git training repository on your local workstation.**

#### Glossary of Terms
<sup>1</sup>**git switch**: This is a relatively new git command introduced in version 2.23 of Git, the
following is a good article on what all it entails: https://www.infoq.com/news/2019/08/git-2-23-switch-restore/

#### [return to demo-02](directions-demo-02.md)
#### [proceed to demo-03](../demo_03/directions-demo-03.md)