#### [return to demo-03](directions-demo-03.md)
# Directions for Atlassian Sourcetree

Open Sourcetree. The software should still have your `branch` checked out. If not, navigate to it,
and check it out.

Unlike some of our other pathways, Sourcetree is not a place to perform the coding work. It is
solely a place for managing your version control. So we'll need to take a slight detour.

In the top ribbon, click **Explorer**, this will open a file explorer window into the directory
of our repository. We'll navigate to the this directory from the root:

- `a-plethora-of-git/demo_03`
- right-click in any of the blank space
    - select **New**
    - select **Text Document**
- name it: *guest-book*
- on line 1
    - add a fun quote
    - sign your name
- **save** your changes

Now that we've made our change we can open Sourcetree back up. You'll see a new entry in the
source... ...tree. It is called `uncommitted` changes. If you'll bring your attention to the bottom
of the screen, we'll review the ways that we can `stage` these changes.

1. **Stage All** - This is mostly fine. Not a great practice, especially if you also have
files in the directory that you don't wanted version controlled. This could include passwords,
configuration files, python notebooks used for testing and prototyping, etc. Generally we are
worried about leaking secrets/passwords. That's why we should be careful about what we `commit`.
2. **Stage Selected** - If you left-click an item you will have access to this button. It allows
you to manually select which files you would like to stage.
3. **+** - This works similar to `2.` and will work on a single file at a time

Now that our file is staged we have a few options:

1. right-click in the **Staged files** section
    - click Commit
2. click the **Commit** button at the top ribbon

This will open the `Commit` panes. At the bottom there is a section with your name / email. This
is where you'll write your commit message.

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

![sourcetree-01.png](../assets/demo-03/sourcetree-01.png)
![sourcetree-02.png](../assets/demo-03/sourcetree-02.png)
![sourcetree-03.png](../assets/demo-03/sourcetree-03.png)
![sourcetree-04.png](../assets/demo-03/sourcetree-04.png)
![sourcetree-05.png](../assets/demo-03/sourcetree-05.png)


***

#### [return to demo-03](directions-demo-03.md)
#### [proceed to demo-04](../demo_04/directions-demo-04.md)