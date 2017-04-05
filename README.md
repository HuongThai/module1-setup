# Module 1: Setting up your Machine

In this course, we'll be using a variety of different software programs to write, manage, and execute the code that we write. Unfortunately, one of the most frustrating and confusing barriers to working with code is simply getting your machine properly set up. This repository aims to provide sufficient information for setting up your machine, and troubleshooting the process. Do your best to follow instructions and search for help online, but don't waste too much time (e.g., more than 15 minutes) before contacting your professor or TA.

Note, classroom machines for this course should have all appropriate software already installed and ready to use.

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Contents**

- [Resources](#resources)
- [Summary](#summary)
- [Git](#git)
  - [GitHub](#github)
- [Command-line Tools (Bash)](#command-line-tools-bash)
  - [Mac](#mac)
  - [Windows](#windows)
- [Python](#python)
  - [Anaconda](#anaconda)
- [Text Editors](#text-editors)
  - [Visual Studio Code](#visual-studio-code)
  - [Atom](#atom)
  - [SublimeText](#sublimetext)
  - [PyCharm](#pycharm)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Resources
The resources for this module are links to recommended software, collected here for easy access.
- [git (and Git Bash)](https://git-scm.com/downloads)
  - [GitHub](https://github.com/join) (sign up)
  - optional: [Bash on Windows](https://msdn.microsoft.com/en-us/commandline/wsl/install_guide)
- [Python (Anaconda)](https://www.continuum.io/downloads)
- [Visual Studio Code](https://code.visualstudio.com/)


## Summary
In short, you'll need to install the following programs: see below for more information / options.
- **Git**: A set of tools for tracking changes to code (especially when collaborating with others). This program is already installed on Macs.

  - **GitHub**: A web service for hosting code online. You don't actually need to _install_ anything GitHub (it uses `git`), but you'll need to sign up for the service.

- **Bash**: A _command-line interface_ for controlling your computer. `git` is a command-line program so you'll need a command shell to use it. Macs already have a Bash program called _Terminal_. On Windows, installing `git` will also install a Bash shell called _Git Bash_, or you can try the (experimental) Linux subsystem for Windows 10.

- **Python**: a general purpose programming language, but one that is often used when working with data. This will be our primary language for the quarter (though we will explore some others as well). "Installing Python" actually means installing tools that will let your computer understand and run Python code.

  - **Anaconda**: is a _distribution_ of the Python language, which includes a large number of additional add-on packages that we will be using (and can be difficult to install on their own). This is the recommended way of installing Python; we will be assuming that you have installed all of tools provided with the distribution.

- **Visual Studio Code**: A lightweight text editor that supports programming in lots of different languages.

  - You are welcome to use another text editor if you wish; some further suggestions are included.


The following sections have additional information about the purpose of each component, how to install it, and alternative configurations.

If you run into any installation/configuration challenges, please let us know on course Slack Channel so that others can anticipate the same issues.

## Git
`git` is a version control system that provides a set of commands that allow you to manage changes to written code, particularly when collaborating with other programmers (much more on this in [module 4](../../../module4-git-basics)). For now, you'll need to [download](https://git-scm.com/downloads) and install the software. Note, if you are using a Windows machine, this will also install a program called Git Bash, which provides a text-based interface for executing commands on your computer. For alternative/additional Windows command-line tools, see below.

### GitHub
GitHub is a website that is used to store copies of code that are being managed with `git` (think "Imgur for code"). These learning modules are on GitHub (check out the URL!). You will also be using GitHub to turn in your programming assignments.

In order to use GitHub, you'll need to [create a free GitHub account](https://github.com/join), if you don't already have one. You should register a username that is identifiable as you (e.g., based on your name or your UW NetID). This will make it easier for us to collaborate and for the teaching staff to figure out who submitted what, rather than needing to figure out who 'LeetDesigner2099' is. This can be the start of a professional account you may use for the rest of your career!

## Command-line Tools (Bash)
The command-line provides a text-based interface for giving instructions to your computer (much more on this in [module 2](../../../module2-command-line)). In this course, we'll use the command-line for navigating our computer's file structure, running programs, and executing commands that allow us to keep track of changes to the code we write (i.e., version control with `git`).

In order to use the command-line, you will need to use a **command shell** (a.k.a. a _command prompt_). This is a program that provides the interface to type commands into. In particular, we'll be working with the <a href="https://en.wikipedia.org/wiki/Bash_(Unix_shell)">Bash</a> shell, which provides a particular set of commands common to Mac and Linux machines.

### Mac
On a Mac you'll want to use the built-in app called **Terminal**. You can open it by searching via Spotlight (hit `Cmd (⌘)` and `Spacebar` together, type in `"terminal"`, then select the app to open it), or by finding it in the `Applications/Utilities` folder.

### Windows
On Windows, we recommend using [Git Bash](https://git-scm.com/downloads), which you should have installed along with `git` (above). Open this program to open the command-shell. This works great, since we'll often be using the command-line for performing version control.

- Note that Windows does come with its own command-prompt, called the _DOS Prompt_, but it has a different set of commands and features. _Powershell_ is a more powerful version of the DOS prompt if you really want to get into the Windows Management Framework. But Bash is more common for the kinds of computer programming that we'll be doing, and so we will be focusing on that set of commands.

Alternatively, the 64-bit Windows 10 Anniversary update (August 2016) _does_ include a beta version of an integrated Bash shell. You can access this by [enabling the subsystem for Linux](https://msdn.microsoft.com/en-us/commandline/wsl/install_guide) and then running `bash` in the command prompt. This is currently (Dec 2016) "beta" technology, but will suffice for our purposes if you can get it running.

## Python
The primary programming language we will use throughout the course is Python. It's a very powerful, general-purpose programming language that is "friendly" enough that it is often used for information and data sciences. However, in order to have the computer run your programs, you will need to install the **interpreter** that the computer uses.

**Important note:** There are two different versions of Python that exist in the world: Python 2 (latest: 2.7) and Python 3 (latest: 3.6). While mostly similar, the newer Python 3 version added [a few basic differences](https://wiki.python.org/moin/Python2orPython3) that make it incompatable with Python 2. But a lot of existing programs were slow to change over to Python 3, effectively causing two different versions to exist in active use (kind of like people not switching from Windows XP). Python 3 is considered the "current" version, with Python 2 being "legacy".

In this course we will be working with **Python 3**. Thus you will want to make sure that you _install_ Python 3, and that documentation and examples you reference is _for_ Python 3 (rather than Python 2)!

### Anaconda
There are a number of ways to get Python installed on your machine: in fact, you may have a version (probably Python 2) installed on your computer already! However, the recommended approach for programming for data science is to install the [**Anaconda**](https://www.continuum.io/downloads). Anaconda is a pre-packaged bundle of common Python tools and packages that are commonly used in data science&mdash;many of which we will be utilizing (including [Jupytr](http://jupyter.org/) for running interactive "notebooks", and [pandas](http://pandas.pydata.org/) for large-scale data work). And the best part: Anaconda makes it easy to get all the pieces installed and ready to use!

To install Anaconda (and Python along with it), simply download the **Python 3.6** installer, run the executable, and follow the instructions. This should install Python and all the required packages.

- You can confirm that everything is set up correctly by opening the _Command Shell_ you installed above and typing `python --version`. You should see text that looks something like:

  ```
  Python 3.6.0 :: Anaconda 4.3.1 (x86_64)
  ```

  confirming that Python is installed and available.


## Text Editors
In order to write code, you need somewhere to write it (we don't want to write it in MS Word!). There are a variety of available programs that provide an interface for editing code. A major advantage of these programs is that they provide automatic formatting/coloring for easier interpretation of the code, along with cool features like auto-completion and integration with version control.

There are lots of different text editors out there, all of which have slightly different appearances and features. You only need to download and use one of the following programs (we recommend **Visual Studio Code** as a default), but feel free to try out different ones to find something you like (and then evangelize about it to your friends!)

### Visual Studio Code
[Visual Studio Code](https://code.visualstudio.com/) (or VS Code; not to be confused with Visual Studio) is an open-source editor developed by Microsoft. While it focuses on web programming and JavaScript, it readily supports lots of languages including Python, and provides a number of [community-built extensions](https://code.visualstudio.com/docs/editor/extension-gallery) for adding even more features. Although fairly new, it is updated regularly and has has become one of my main editors for programming.

Click the "Download" button to download the installer (e.g, `.exe`) file, then double-click on that to install the application.

Once you've installed VS Code, the trick to using it effectively is to get comfortable with the [Command Palette](https://code.visualstudio.com/docs/getstarted/userinterface#_command-palette). If you hit `Cmd+Shift+P`, VS Code will open a small window where you can search for whatever you want the editor to do. For example, if you type in `markdown` you can get list of commands related to Markdown files (including the ability to open up a preview).

- While VS Code can handle Python code just fine out of the box, to be most effective when writing code you'll want to add an extension with [additional Python support](https://code.visualstudio.com/docs/languages/python). We recommend [Don Jayamanne's](https://marketplace.visualstudio.com/items?itemName=donjayamanne.python) extension: you can easily install this by using the command-palette (open it up and type `"extension"` to find the "Install Extensions" option). Note that you can disable the pervasive "style warnings" by adding `# pylint: skip-file` to the top of a script file.

For more information about using VS Code, see [the documentation](https://code.visualstudio.com/docs), which includes [videos](https://code.visualstudio.com/docs/getstarted/introvideos) if you find them useful.

### Atom
[Atom](https://atom.io/) is a text editor built by the folks at GitHub and has been gaining in popularity. It is very similar to VS Code in terms of features, but has a somewhat different interface and community. It has a similar command-palette to VS Code, and is arguably even nicer about editing Markdown specifically (its built-in spell-check is a great feature, especially for documents that require lots of written text). The document you are reading was authored in Atom.

### SublimeText
[SublimeText](https://www.sublimetext.com/3) is a very popular text editor with excellent defaults and a variety of available extensions (though you'll need to manage and install extensions to achieve the functionality offered by other editors out of the box). While the software can be used for free, every 20 or so saves it will prompt you to purchase the full version. This is my application of choice for when I just write to write a plain text file.

### PyCharm
[PyCharm](https://www.jetbrains.com/pycharm/) is a full-featured Python IDE (integrated development environment) developed by JetBrains. It has more features than you can shake a stick at, including a large number of features that won't be relevant for us. It is more powerful, but also somewhat "heavier" (read: slower). You would be interested in the _Community Edition_ of the software.
