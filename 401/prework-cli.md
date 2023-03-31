# Bash Command Line Tutorials Summary

## Introduction to the Command Line

- A command line interface (CLI) is a textual way of interacting with a computer.
- Bash is the most common Unix shell in Linux environments.
- CLI is more powerful and efficient for certain tasks, especially for automation.
- To access the command line, open a terminal in Linux, or use a terminal emulator like PuTTY for Windows.

## Navigation

- Linux uses a hierarchical directory structure with `/` as the root directory.
- Essential directories: `/home` (user directories), `/etc` (configuration files), `/var` (variable data), `/bin` and `/sbin` (system executables).
- `pwd` displays the current working directory.
- `cd` changes the current directory.
- `ls` lists the contents of a directory with optional flags for extra information, like `ls -l` for long format or `ls -a` for hidden files.

## About Files

- Everything in Linux is a file, including directories, devices, and sockets.
- File types: regular files, directories, symbolic links, block and character devices, and sockets.
- File extensions are not enforced but provide useful information about file contents.
- Permissions: read, write, and execute for user, group, and others, displayed as `rwxrwxrwx`.
- `chmod` command can change permissions, and `chown` changes ownership.
- Wildcards like `*` and `?` help to match multiple files at once.

## Manual

- Man pages (short for manual pages) provide documentation for most Linux commands.
- Access man pages with `man <command>`.
- Man pages are divided into sections (e.g., User Commands, System Calls, Library Functions).
- Use `whatis` for a brief description of a command, and `apropos` to search man pages for a keyword.

## File Manipulation

- `touch` creates new, empty files or updates timestamps on existing files.
- `mkdir` creates directories, and `rmdir` removes empty directories.
- `cp` copies files and directories with `-r` flag for recursive copying of directories.
- `mv` moves files and directories or renames them.
- `rm` removes files, with the `-r` flag to delete directories recursively.
- `ln` creates hard or symbolic links with `-s` flag for symbolic links.

_Ah-hah moments_:

1. Realizing that everything in Linux is treated as a file simplifies understanding of the system and allows for unified operations.
2. The power of wildcards to operate on multiple files at once is extremely useful for batch operations and automation.
3. The availability of man pages for almost every command is an invaluable resource for learning and troubleshooting.

_Interesting code snippets_:

1. `ls -lh` combines the long format with human-readable file sizes.
2. `chmod u+x filename` adds execute permission to the user for a specific file.
3. `cp -R /path/to/source /path/to/destination` copies a directory and its contents to a new location.

## [Cheatsheet](https://ryanstutorials.net/linuxtutorial/cheatsheet.php)
