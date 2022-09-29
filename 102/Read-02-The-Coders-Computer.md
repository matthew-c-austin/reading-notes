# Choosing a Text Editor
## What is a Text Editor?
A text editor is a piece of software that you download and install on your computer, or you access online through your web browser, that allows you to write and manage text. Word processers like Microsoft Word is technically a text editor. In the world of programming, we look at types of text editors called code editors.

Important features to look for in a text editor:
- Code Completion
- Syntax highlighting
- A variety of themes (to reduce eye strain and fatigue)
- The ability to choose from a healthy selection of extensions, when needed

## Text Editor Options

You can either use software that comes with your O/S, such as "Text Edit" on Mac or "Notepad" on Windows. For Linux computers, each distribution will have its own text editor already installed but which one might depend on the flavor of your particular distribution. These text editors will go by different names. One distro might have “Gedit,” and others might have other titles. Check you list of applications to see which text editor comes with your distribution of Linux.

However, most of these are extremely bare bones when it comes to features, i.e., none of the sought after features listed above. There are several better third party options

### Notepad ++

Notepad++ is a free editor for Windows computers only. It's been aroun dfor years and many devs swear by it. Some notable features are syntax highlighting and code
completion, as well as word completion and function completion. It has a zoom in an out feature, it’s own online community, and its own chat room for questions that may arise. It even has its own searchable wiki page for more assistance.

### TextWrangler/BB Edit

TextWrangler is a Mac only text editor, which has since been retired (back in 2017). The company that owns it, Bare Bones Software, has incorporated TextWrangler into a more robust editor, BB Edit. BB Edit is software that you purchase. But BB Edit comes with a 30-day free trial. After the 30 days is over, if you still want the free version, simply continue using BB Edit, and you’ll get the same features as you would have gotten in TextWrangler. 

### Visual Studio Code

Visual Studio Code is a free text editor made by the folks at Microsoft. It is available for Windows computers, Mac computers and Linux computers. VS Code has the Emmet shorthand for HTML and CSS already built-in with no additional work from you at all. VS Code has everything: syntax highlighting, themes, extensions and code
completion. It seems like VS Code has a very healthy following in the web developing community.

### Atom

Atom is GitHub's text editor, and it's available for Windows, Mac, and Linux computers. It has syntax highlighting, themes, extensions, etc.

### Brackets

Brackets is a free text editor made by Adobe. Those two words, free and Adobe, don't really ever go together in a sentence. However, Brackets is free and it supports HTML, CSS, and JavaScript.

### Sublime Text

Sublime Text 3 is a premium software that can be purchased in full for $70. Otherwise you’ll use the free version. Sublime Text enjoys a history of being fast and responsive while being extensible as well. There’s no doubt that Sublime Text will tick the check boxes of what to look for in a text editor. It has syntax highlighting, it has code completion, it has themes and extensions.

## The Difference Between Text Editors and IDEs

An IDE (Integrated Development Environment) is really a suite of different software all coming together. An IDE is a text editor, a file manager, a compiler, and a debugger all in one software package. The difference really is that an IDE is an all-in-one software package. There are dozens of IDEs as well, and this link has them broken up by software language, with notable differences: [IDE Comparison](https://en.wikipedia.org/wiki/Comparison_of_integrated_development_environments)


# The Terminal AKA: The Command Line Interface (CLI)

[Linux Tutorial: The Command Line!](https://ryanstutorials.net/linuxtutorial/commandline.php)

The terminal is able to do everything that a file explorer can do. However, instead of using a mouse and visualization for navigation and manipulation of files, it all takes place in a purely textual window.

A command line, or terminal, is a text based interface to the system. You are able to enter commands by typing them on the keyboard and feedback will be given to you similarly as text.

## The Shell

Within a terminal you have what is known as a shell. This is a part of the operating system that defines how the terminal will behave and looks after running (or executing) commands for you. There are various shells available but the most common one is called bash which stands for Bourne again shell. This tutorial will assume you are using bash as your shell.

If you would like to know which shell you are using you may use a command called echo to display a system variable stating your current shell. echo is a command which is used to display messages.

## Useful and Common Commands

- pwd : print working directory (you are here)
- ls : list
  - ls -l : list with more information as a list
  - ls -a : list with hidden files
- cd <directory> : change directory to <directory>
   - cd . : go up one level (or .. for two, ... for three etc.)
- mkdir <directory> : make a directory
- touch <file.ex> : make an empty file with name file and extension .ex

For more useful and common commands, see [Linux CLI Cheat Sheet](https://ryanstutorials.net/linuxtutorial/cheatsheet.php)
  
### Tab Completion
  
When you start typing a path (anywhere on the command line, you're not just limited to certain commands) you may hit the Tab key on your keyboard at any time which will invoke an auto complete action. If nothing happens then that means there are several possibilities. If you hit Tab again it will show you those possibilities. You may then continue typing and hit Tab again and it will again try to auto complete for you.

## Navigation
  
This section is about the basics of moving around in the system.
  
### Paths
  
There are 2 types of paths we can use, absolute and relative. Whenever we refer to a file or directory we are using one of these paths. Whenever we refer to a file or directory, we can, in fact, use either type of path (either way, the system will still be directed to the same location).

To begin with, we have to understand that the file system under linux is a hierarchical structure. At the very top of the structure is what's called the root directory. It is denoted by a single slash ( / ). It has subdirectories, they have subdirectories and so on. Files may reside in any of these directories.

Absolute paths specify a location (file or directory) in relation to the root directory. You can identify them easily as they always begin with a forward slash ( / )

Relative paths specify a location (file or directory) in relation to where we currently are in the system. They will not begin with a slash.

You'll find that a lot of stuff in Linux can be achieved in several different ways. Paths are no different. Here are some more building blocks you may use to help build your paths.

- ~ (tilde) - This is a shortcut for your home directory. eg, if your home directory is /home/ryan then you could refer to the directory Documents with the path /home/ryan/Documents or ~/Documents
- . (dot) - This is a reference to your current directory. eg in the example above we referred to Documents on line 4 with a relative path. It could also be written as ./Documents (Normally this extra bit is not required but in later sections we will see where it comes in handy).
- .. (dotdot)- This is a reference to the parent directory. You can use this several times in a path to keep going up the hierarchy. eg if you were in the path /home/ryan you could run the command ls ../../ and this would do a listing of the root directory.
  
### Miscellany
  
Some interesting paths:
  
- /etc - Stores config files for the system.
- /var/log - Stores log files for various system programs. (You may not have permission to look at everything in this directory. Don't let that stop you exploring though. A few error messages never hurt anyone.)
- /bin - The location of several commonly used programs (some of which we will learn about in the rest of this tutorial.
- /usr/bin - Another location for programs on the system.
  
## More About Files

### Oops all Files
  
The first thing we need to appreciate with linux is that under the hood, everything is actually a file. A text file is a file, a directory is a file, your keyboard is a file (one that the system reads from only), your monitor is a file (one that the system writes to only) etc. To begin with, this won't affect what we do too much but keep it in mind as it helps with understanding the behaviour of Linux as we manage files and directories.

### An Extensionless System
  
This one can sometimes be hard to get your head around but as you work through the sections it will start to make more sense. A file extension is normally a set of 2 - 4 characters after a full stop at the end of a file, which denotes what type of file it is. The following are common extensions:

- file.exe - an executable file, or program.
- file.txt - a plain text file.
- file.png, file.gif, file.jpg - an image.
  
In other systems such as Windows the extension is important and the system uses it to determine what type of file it is. Under Linux the system actually ignores the extension and looks inside the file to determine what type of file it is.
  
### Case Sensitivity and Naming

This is very important and a common source of problems for people new to Linux. Other systems such as Windows are case insensitive when it comes to referring to files. Linux is not like this. As such it is possible to have two or more files and directories with the same name but letters of different case.

Spaces in file and directory names are valid, but should be used with caution. Since spaces are how items on the command are separated, typing Holiday Photos as the directory wouldn't work for the cd command. You should either use:

- Quotes : 'Holiday Photos' or "Holiday Photos"
- Escape Characters : Holiday\ Photos (the backslash nullifies the special meaning of the whitespace character)

Linux actually has a very simple and elegant mechanism for specifying that a file or directory is hidden. If the file or directory's name begins with a . (full stop) then it is considered to be hidden. You don't even need a special command or action to make a file hidden. Files and directories may be hidden for a variety of reasons. Configuration files for a particular user (which are normally stored in their home directory) are hidden for instance so that they don't get in the way of the user doing their everyday tasks.
