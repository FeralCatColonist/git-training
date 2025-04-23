#### [return to demo-03](directions-demo-03.md)
# Directions for Visual Studio Code

Open your repository directory in Visual Studio Code.

We have a few options for creating a new file.

1. In the **Explorer** pane, move your cursor on top of the directory entry for `demo_03` you
can right-click and click **New File...**

- a new file entry will appear in the **Explorer** pane
    - name it guest-book.txt
- the file will automatically open in a new tab

2. Click **File** on the top tab, for this demo, you can select either **New Text File** or **New File** by default,
these files are named Untitled-X and not saved, after making changes, you must manually save them.

- **New Text File** will open a new tab
- **New File** will open the **Command Palette** and prompt you to select a file type
    - these options will differ depending on the context of the directory you are in and the extensions
    you have installed
    - select **New Text File**

- press `ctrl + s` to save, the save dialog box will appear
    - save the file as guest-book.txt within at `git-training\a-plethora-of-git\demo_03` directory
    - on the first line type a phrase and sign your name
        - be sure to save your work, a white dot will appear in the tab name if it is currently un-saved

You'll notice the **Source Control** pane will now have a blue icon with the number 1 on it. This is a counter of the
number of changes that have been made to the repository.

- Click the **Source Control** pane
- In the top left you'll see a small section with the word **Changes** above it
    - beneath this section is a text box
    - beneath this text box is a large, blue button with a **check mark** and the word **Commit**
- beneath that button you'll see a section called **Staged Changes**
- beneath the **Staged Changes** section is an additional section, **Changes**
    - in this section, you'll see the file we just created `guest-book.txt`
- click the **+** button to move this file into the **Staged Changes** section
    - or right click and select **Stage Changes**

Now that we've staged our changes, we're ready to write a `commit message` and `commit` these changes.

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

- write your `commit` message
- click **Commit** 

**You have officially made your first commit!**

#### [return to demo-03](directions-demo-03.md)
#### [proceed to demo-04](../demo_04/directions-demo-04.md)

***

![vs-code01.png](../assets/demo-03/vs-code01.png)
![vs-code02.png](../assets/demo-03/vs-code02.png)
![vs-code03.png](../assets/demo-03/vs-code03.png)
![vs-code04.png](../assets/demo-03/vs-code04.png)

***

#### [return to demo-03](directions-demo-03.md)
#### [proceed to demo-04](../demo_04/directions-demo-04.md)