#### [return to demo-06](directions-demo-06.md)
# Directions for Git for Windows

Open Git Bash and navigate to the repository directory.

> - create a new `branch`
>     - it can be based on main or your other branch that was submitted as a pull request
>     - name it something like `jcarmona-branch-cleaning`
> - create a new file within the demo_06 directory
> - commit the change
> - push the change to Bitbucket
> - navigate to the **Branches** section of the repository within Bitbucket
> - find your new `branch`
>     - click the **...** in the **Actions** column
>     - click **Delete**

Our local `branch` no longer has an upstream counterpart. Assuming we do not have any *new* commits left
in our `branch` we can use the following command, *after*, we switch to an active `branch` like main:

```bash
git fetch --prune
```

This:

- downloads commits, files, and references
- removes local branches that are tracked remotely when the remote `branch` no longer exists on the
remote repository

**Congratulations! You have pruned a local branch and kept your workspace tidy.**

#### [return to demo-06](directions-demo-06.md)

***

![bitbucket-01.png](../assets/demo-06/bitbucket-01.png)
![git-for-windows-01.png](../assets/demo-06/git-for-windows01.png)

***

#### [return to demo-06](directions-demo-06.md)