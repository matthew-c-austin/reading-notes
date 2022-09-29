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
