#### [return to demo-06](directions-demo-06.md)
# Directions for Atlassian Sourcetree

Open Sourcetree.

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

- click the **Fetch** button
- in the **Fetch** dialog box
    - select Fetch from all remotes
    - select Prune tracking branches no longer present on remote(s)
- this should work, but doesn't
    - https://jira.atlassian.com/browse/SRCTREEWIN-8426

Instead, let's do the following:

- right click your new `branch`
- click **Delete your-branch-name**

**Congratulations! You have pruned a local branch and kept your workspace tidy.**

#### [return to demo-06](directions-demo-06.md)

***

![bitbucket-01.png](../assets/demo-06/bitbucket-01.png)
![sourcetree-01.png](../assets/demo-06/sourcetree-01.png)
![sourcetree-02.png](../assets/demo-06/sourcetree-02.png)

***

#### [return to demo-06](directions-demo-06.md)