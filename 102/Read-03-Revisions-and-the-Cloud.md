# Git Tutorial

[Udemy Blog](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/#7_2)

## Version Control

Version control is a system that allows you to revisit various versions of a file or set of files by recording changes. With it, you can revert a file or project to a previous version, track modifications and individuals who make modifications, and compare changes. Utilizing a Version Control System (VCS) allows for mistakes to be easily rectified.

### Local Version Control

Like it sounds, Local VCS entails one database on a hard disk that stores changes to files.

### Centralized Version Control

The need for collaboration between developers on a team led to the advent of the Centralized Version Control System (CVCS). This entails a single server storing all changes and file versions, which can be accessed by various clients. This eliminates the need to involve all local databases, streamlining the collab process and allowing programmers to have more knowledge of team members' activities with certain files, as well as giving admins more control by divvying up revision privileges.

### Distributed Version Control

A Distributed Version Control System (DVCS) addresses the major vulnerability of the CVS: the server as a single point of failure. If a CVS goes down, collaboraters can't work with each other on file changes and new versions. Also, in the event of corruption to the database's hard disk, and with an absence of backups, all work is lost.

To prevent this type of loss, a DVCS allows clients to create mirrored repositories. These data backups can easily be placed on the server to replace any lost information. Because the DVCS allows for multiple mirrored repos, programmers can collaborate with each other in various ways to complete a joint project, which enables the use of simultaneous workflows.

## What is Git?

Git is a DVCS that stores data in a file system made up of **snapshots**. Each time you save a changed version of your project — called **commit** — Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.

Git mostly relies on local operations because most info can be found there, and quickly - since it doesn't need to fetch history information from a server. This also allows for the continued work on a project when not online or on a VPN.

Every single change applied to any file or directory is tracked by Git. As the gatekeeper, Git always detects file corruption or loss of information in transit.

### States

Files in Git can reside in three main states: commited, modified, and staged.

- **Committed**: Data is securely stored in a local database
- **Modified**: File has been changed but not commited to the database
- **Staged**: Flagged a file's changed version to be committed in the next snapshot

![Git States](https://blog.udemy.com/wp-content/uploads/2015/08/image066.png)

### History of Git

Git traces its roots to the open source software project Linux kernel. Subsequently, Linus Torvalds, the chief architect of the Linux kernel, began creating Git. With the intention of creating a DVCS with a workflow design similar to that of BitKeeper, which was also fast, Git allowed for non-linear development via multiple branches, could support large projects, possessed strong mechanisms preventing corruption, and had a simple design.

### Setting up Git

An inherent Git tool called `git config` allows the setting of configuration variables that control aspects of Git’s operation and look.

To check settings, use the `git config --list` command.

There are three ways to get more information on a particular command, by accessing the manual:

`git help command`

`git command --help`

`man git-command`

### Setting up a Git Repository

#### Importing

To import an existing project directory into Git, follow these steps using the CLI:

1. Switch to the target project's directory
2. Use the git init command `git init`
3. To start tracking these repo files, perform an initial commit by typing the following:

`git add *.c`

`git add LICENSE`

`git commit -m "any message here"`

Now, your files are tracked and there’s an initial commit.

#### Cloning

You can also create a copy of an existing Git repo using hte clone command:

`git clone https://github.com/test`

To clone a repo into a directory with another name of your choosing, use:

`git clone https://github.com/test mydirectory`

The command above makes a copy of the target repository in a directory named “mydirectory.”

### Workflow

#### Local Repository Structure

The local Git repo has three components:

1. Working Directory: The actual files reside here.
2. Index: The area used for staging
3. Head: Points to the most recent commit

#### Saving Changes

All files in a checked out (or working) copy of a project file are either in a tracked or untracked state.

**Tracked** - Tracked files can be modified, unmodified, or staged; they were part of the most recent file snapshot.

**Untracked** - Untracked files were not in the last snapshot and do not currently reside in the staging area.

#### The Life Cycle of File Status

1. After you edit a file, Git flags it as modified because of changes made after the previous commit.
2. You stage the modified file.
3. Then, you commit staged changes.

![life cycle](https://blog.udemy.com/wp-content/uploads/2015/08/image006.png)

#### Check File Status

`git status`

#### Tracking and Staging a New File

Single File

`git add filename`

All Files

`git add *`


#### Committing a File

`git commit -m “made change x,y,z”` - This step has committed changes for the file or files (you can have one commit message for multiple files, if applicable) to the HEAD.

#### Committing All Changes

`git commit -a`

#### Pushing Changes

`git push origin master` - For cloned repositories, Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local repository. However, these names can be changed by the user.

#### Stashing Changes

 `git stash` - This command temporarily removes changes and hides them, giving you a clean working directory.

 `git stash apply`- Retrieve the hidden changes.

### Remote Repositories

In order to collaborate on Git projects, you must interact with remote repositories, versions of a project residing online or on a network. You can work with multiple repositories, for which you can have read/write or read-only privileges. Teams can use remote repositories to push information to and pull data from.

#### Cloned Repositories

Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local branch.

#### Seeing Your Remotes

By running the `git remote` command, you can view the short names, such as “origin,” of all specified remote handles.

By using `git remote -v`, you can view all the remote URLs next to their corresponding short names.

