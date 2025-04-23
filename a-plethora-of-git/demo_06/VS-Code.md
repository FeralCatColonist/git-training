#### [return to demo-06](directions-demo-06.md)
# Directions for Visual Studio Code

Open Visual Studio Code and the directory where the local repository is stored.

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

- type `ctrl + shift + p` to enter the **Command Palette**
- type `git prune`
    - depending on the extensions you have installed you will see multiple options

You can select either:

- **Git: Fetch (Prune)** if using only VS Code's Source Control
    - click the option within the **Command Palette**
- **GitLens: Prune Branches...**
    - select your named `branch`
    - click **OK**
    - click **Delete Branch**

**Congratulations! You have pruned a local branch and kept your workspace tidy.**

#### [return to demo-06](directions-demo-06.md)

***

![bitbucket-01.png](../assets/demo-06/bitbucket-01.png)
![vscode-01.png](../assets/demo-06/vscode-01.png)
![vscode-02.png](../assets/demo-06/vscode-02.png)
![vscode-03.png](../assets/demo-06/vscode-03.png)

***

#### [return to demo-06](directions-demo-06.md)