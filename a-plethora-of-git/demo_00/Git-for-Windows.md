#### [return to demo-00](directions-demo-00.md)
# Directions for Git for Windows

![Git for Windows Logo](../assets/logo-git-for-windows.png){width=200px}

> Git for Windows focuses on offering a lightweight, native set of tools that bring the full feature
> set of the Git SCM<sup>1</sup> to Windows while providing appropriate user interfaces for experienced
> Git users and novices alike.
\- [Git for Windows](https://gitforwindows.org/)

Proceed to the shared software installation folder: `\\some-network-path`

The following is a step-by-step guide for the installation process:

### Step 1: Launching the Installer
1. Double-click on the installer file `Git-2.48.1-64-bit.exe`

### Step 2: License Information
The Git for Windows installer should now launch and display the license information screen.

1. Click the **Next** button to accept the license and proceed

### Step 3: Installation Location
After accepting the license, you'll see the installation location selection screen. The default
installation directory is generally appropriate. You can change this location by clicking the
**Browse** button if needed.

1. Click **Next** to continue to the component selection screen.

### Step 4: Select Components
After choosing the installation location, you'll see the component selection screen.

1. The following is a list of default components that are pre-selected:
    - Windows Explorer integration
    - Git Bash
    - Git GUI
    - Git LFS (Large File Support)
    - Associate Git files with default editor

2. I would recommend selecting all the options except possibly adding an icon to the desktop

### Step 5: Choosing Default Editor
After selecting components, you'll see the default editor selection screen.

1. In the drop-down menu, select Use Visual Studio Code as Git's default editor
2. Click **Next** to continue to the branch naming convention screen.

### Step 6: Initial Branch Name Configuration
After selecting your default editor, you'll see the initial branch name configuration screen.

1. Select the second option: Override the default branch name for new repositories

    - we'll enter the term `main` as our standard

2. Click **Next** to continue to the PATH environment configuration.

### Step 7: Adjusting PATH Environment
After setting the default branch name, you'll see the PATH environment configuration screen.

1. We'll utilize the middle, recommended option:

    - Git from the command line and also from 3rd-party software
    
2. Click Next to continue to the HTTPS transport backend configuration.

### Step 8: HTTPS Transport Backend Configuration
After configuring the PATH environment, you'll see the HTTPS transport backend selection screen.
For most users in an organization-managed environment (like us), the recommendation is to use the
second option.

1. Select: Use the native Windows Secure Channel library
2. Click Next to continue to the line ending configuration.

### Step 9: Line Ending Configuration
After selecting the HTTPS transport backend, you'll see the line ending configuration screen.
For most Windows users, the first option (default) is recommended for best compatibility.

1. Select: Checkout Windows-style, commit Unix-style line endings
2. Click **Next** to continue to the terminal emulator configuration.

### Step 10: Terminal Emulator Configuration
After configuring line endings, you'll see the terminal emulator configuration screen.
For most users, the default MinTTY option provides a better experience.

1. Select: Use MinTTY (the default terminal of MSYS2)
2. Click **Next** to continue to the default behavior for `git pull` configuration.

### Step 11: Default Behavior for Git Pull
After selecting the terminal emulator, you'll see the default behavior for `git pull` configuration screen.
For beginners, the default option is typically easiest to work with.

1. Select: Default (fast-forward or merge)
2. Click **Next** to continue to the credential helper configuration.

### Step 12: Credential Helper Configuration
After configuring the default git pull behavior, you'll see the credential helper configuration screen.

1. Select: Git Credential Manager
2. Click **Next** to continue to the extra options configuration.

### Step 13: Extra Options Configuration
After configuring the credential helper, you'll see the extra options configuration screen.

1. Select: Enable file system caching
2. Likely, you will not need additional features here.

### Step 14: Installation and Completion
Once the installation completes, you'll see a completion screen with options to launch Git Bash and
view release notes.

1. Check "Launch Git Bash" if you want to immediately test your installation
2. Click **Finish** to complete the installation

You will also need access to the Bitbucket, if you haven't already, ensure you browse to the following
URL:

- **https://bitbucket.org/some-tenant/workspace**

If you don't have access, let us know and we'll send an invite to your organization email.

#### Glossary of Terms
<sup>1</sup>**SCM:** Source Code Management

#### [return to demo-00](directions-demo-00.md)
#### [proceed to demo-01](../demo_01/directions-demo-01.md)