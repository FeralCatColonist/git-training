#### [return to demo-03](directions-demo-03.md)
# Directions for Git for Windows

Open Git Bash. Enter the following commands:

```bash
cd "the-path-to-your-directory/git-training/a-plethora-of-git/demo_03"
# enter a phrase and sign your name
echo '"Hello World!" - Jordan Carmona' > guest-book.txt
```

This:

- changes the directory (folder) the bash terminal is pointed to
    - to the subdirectory `demo_03`
- prints the text `"Hello World!" - Jordan Carmona` into a file called `guest-book.txt`

Alternatively, we can use the built-in Nano editor:

```bash
cd "the-path-to-your-directory/git-training/a-plethora-of-git/demo_03"
nano guest-book.txt
```

- Nano will open
    - type in a phrase, then sign your name
    - enter `ctrl + s` to *save*
    - enter `ctrl + x` to *exit* Nano

Now that we have recorded a change in our repository. Let's see what that looks like.

```bash
git status
```

The terminal will output your current `branch`, it's status against the `origin`, and files that are:

- Changes to be committed
- Changes not staged for commit
- Untracked files

Let's `add` your file to changes to be commited:

```bash
git add guest-book.txt
```

Next we need to `commit` this change. We have some options, but first. 

> Let's talk about the commit message, like `branch` names, we haven't decided upon a set of
> standards yet. There is quite a lot to consider, there are many different opinions, consider
> the following:
> 
> - https://cbea.ms/git-commit/
> - https://www.freecodecamp.org/news/how-to-write-better-git-commit-messages/
> - https://arialdomartini.wordpress.com/2012/09/03/pre-emptive-commit-comments/
> - https://www.chiark.greenend.org.uk/~sgtatham/quasiblog/commit-messages/
>
> That said, imagine you open a Python script and it's just horrible. Really ragged. You're
> honestly embarrassed:
>
> 1. how bad it is 
> 2. you have to work on it
>
> Git blame shows you the original author of this code:
>
> - You.
>     - from six months ago
> ![git-blame01.png](../assets/demo-03/git-blame01.png){width=200px}
> 
> Now if you're asking yourself, literally, "why did you do this!?!" Your commit message
> might tell you everything you need to know. Or it might be useless.
> For now, it's up to you.

As we were saying, we have two options:

1. we can perform the full commit from the git bash terminal like
    - `git commit -m "some commit title" -m "some commit message"`
2. we can `commit` from the terminal, like
    - `git commit`
    - the git bash terminal will open the linked/associated editor
        - with the instructions from `demo-00` this will open VS Code
    - VS Code will open with a new tab
        - type in your commit message
        - save the file, you can use `ctrl + s`
        - close the tab

**You have officially made your first commit!**

#### [return to demo-03](directions-demo-03.md)
#### [proceed to demo-04](../demo_04/directions-demo-04.md)

***

![git-for-windows-01.png](../assets/demo-03/git-for-windows-01.png)
![git-for-windows-02.png](../assets/demo-03/git-for-windows-02.png)
![git-for-windows-03.png](../assets/demo-03/git-for-windows-03.png)
![git-for-windows-04.png](../assets/demo-03/git-for-windows-04.png)

***

#### [return to demo-03](directions-demo-03.md)
#### [proceed to demo-04](../demo_04/directions-demo-04.md)