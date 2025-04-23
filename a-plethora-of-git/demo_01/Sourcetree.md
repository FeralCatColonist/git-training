#### [return to demo-01](directions-demo-01.md)
# Directions for Atlassian Sourcetree

We have two options for creating a Git Clone with Atlassian Sourcetree.

### With Bitbucket
On the repository's page within Bitbucket:
- https://bitbucket.org/some-tenant/git-training/src/main/

Click the `Clone` button on the top right of the page
Then click **Clone in Sourcetree**
This opens the Clone dialogue within Sourcetree, directions below

### With Sourcetree
Open Atlassian Sourcetree. By default the opening screen will list a number of repositories in alpha-order; however,
these repositories are not loaded in alpha-order, you'll need to either:

- scroll to the bottom of the list and click "load more"
- type in the name of the repository "git-training"

Once you have selected the repository, there is only one option, `clone`. Clicking this opens a new context screen:

![../assets/demo-01/atlassian-sourcetree-clone-context-menu.png]

The following items get pre-populated: 

1. The remote repository path it should look like: `user@bitbucket.org/organization-tenant/repository-name.git`
2. Path to the directory on your workstation that you want to `clone` the repository into
3. Bookmark name (within the Sourcetree GUI), by default, takes the name of the directory / repository
    - will also appear as the tabbed name 
4. Local Folder<sup>2</sup>, you can likely ignore this
5. Selection drop-down for different branches within a repository

Click `clone`. Sourcetree will spin for a bit and then complete the process. 

**You now have a local copy of the repository on your workstation.** While it is intended to be viewed within the
Sourcetree software, you can browse to the directory in file explorer by:

6. Clicking the hamburger button (this is the bookmarks bar), right clicking the bookmark, and selecting "Show in Explorer"
7. Clicking the Explorer button

![atlassian-sourcetree-cloned.png](../assets/demo-01/atlassian-sourcetree-cloned.png)


#### Glossary of Terms
<sup>1</sup>**Clone Depth:** the number of commits to be pulled, the default is typically fine: 
- https://community.atlassian.com/forums/Bitbucket-questions/clone-depth-does-what-Why-do-I-care-about-this-setting/qaq-p/496247

<sup>2</sup>**Local Folder:** should probably be called bookmarks: 
- https://community.atlassian.com/forums/Sourcetree-questions/In-Sourcetree-Clone-what-is-the-significance-of-quot-Local/qaq-p/1554736

#### [return to demo-01](directions-demo-01.md)
#### [proceed to demo-02](../demo_02/directions-demo-02.md)