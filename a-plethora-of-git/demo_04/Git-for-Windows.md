#### [return to demo-04](directions-demo-04.md)
# Directions for Git for Windows

Open Git Bash.

> - in demo-02 we created a local `branch`
> - in demo-03 we commited a file to that local `branch`
>
> However, we did not create a remote counterpart of that `branch`. Meaning, that work only exists locally, on our
> workstation. We will perform a `push` operation against our local `branch`, creating a paired copy in the remote
> repository. The result is that we will have a copy of our `branch` locally and on our remote repository on Bitbucket.

Enter the following commands:

```bash
cd "the-path-to-your-directory/git-training"
git push -u origin jcarmona-git-demo
```

This:

- changes the directory (folder) the bash terminal is pointed to
- the `-u` flag is short for `--set-upstream-to`
    - this is a relationship, the assumption is that the upstream `branch` is/should be authoritative
    - the parameter `origin` is a short-hand reference to the remote repository
    - the final parameter is the name we want to give to the remote `branch`

Altogether, this command creates a `branch` named the same as our local `branch` in the remote repository,
and copies the contents of our local branch to it.

> We can review that the operation was successful by navigating to the remote repository:
> 
> - https://bitbucket.org/some-tenant/git-training/src/main/
> 
> Click the drop-down button that says **main**, you will see the name of your `branch` you made locally:
> 
> - click your branch name to change to it
>     - notice this changes the bitbucket URL
> - navigate to the demo-03 directory and you'll find your *guest-book.txt* file

**You have officially pushed your first commit!**

#### [return to demo-04](directions-demo-04.md)
#### [proceed to demo-05](../demo_05/directions-demo-05.md)

***

![git-for-windows-01.png](../assets/demo-03/git-for-windows-01.png)
![git-for-windows-02.png](../assets/demo-03/git-for-windows-02.png)
![git-for-windows-03.png](../assets/demo-03/git-for-windows-03.png)
![git-for-windows-04.png](../assets/demo-03/git-for-windows-04.png)

***

#### [return to demo-04](directions-demo-04.md)
#### [proceed to demo-05](../demo_05/directions-demo-05.md)