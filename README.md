# Module 1: Setting up your Machine

In this course, we'll be using a variety of different software programs to write, manage, and execute the code that we write. Unfortunately, one of the most frustrating and confusing barriers to working with code is simply getting your machine properly set up. This repository aims to provide sufficient information for setting up your machine, and troubleshooting the process. Do your best to follow instructions and search for help online, but don't waste too much time (e.g., more than 15 minutes) before contacting your TA. We'll also set aside time in the first lab session to help with machine set-up.

Note, classroom machines for this course should have all appropriate software already installed and ready to use.

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->


- [Resources](#resources)
- [Summary](#summary)
- [Git](#git)
  - [GitHub](#github)
- [Command-line Tools (Bash)](#command-line-tools-bash)
  - [Mac](#mac)
  - [Windows](#windows)
- [Text Editors](#text-editors)
  - [Atom](#atom)
  - [Visual Studio Code](#visual-studio-code)
  - [SublimeText](#sublimetext)
- [RStudio](#rstudio)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Resources
The resources for this module are links to recommended software, collected here for easy access.
- [git (and Git Bash)](https://git-scm.com/downloads)
  - [GitHub](https://github.com/join) (sign up)
  - optional: [Bash on Windows](https://msdn.microsoft.com/en-us/commandline/wsl/install_guide)
- [Atom](https://atom.io/)
- [RStudio](https://www.rstudio.com/products/rstudio/download3/)
  - [R](https://cran.rstudio.com/) (if required)


## Summary
In short, you'll need to install the following programs: see below for more information / options.
- **Git**: A set of tools for tracking changes to code (especially when collaborating with others). This program is already installed on Macs.

  - **GitHub**: A web service for hosting code online. You don't actually need to _install_ anything GitHub (it uses `git`), but you'll need to sign up for the service.

- **Bash**: A _command-line interface_ for controlling your computer. `git` is a command-line program so you'll need a command shell to use it. Macs already have a Bash program called _Terminal_. On Windows, installing `git` will also install a Bash shell called _Git Bash_, or you can try the (experimental) Linux subsystem for Windows 10.

- **Atom**: A lightweight text editor that supports programming in lots of different languages.

  - You are welcome to use another text editor if you wish; some further suggestions are included.

- **R**: a programming language commonly used for working with data. This will be our primary language for the quarter. "Installing R" actually means installing tools that will let your computer understand and run R code.

- **RStudio**: An graphical editor for writing and running R code. This will soon become our primary development application.

The following sections have additional information about the purpose of each component, how to install it, and alternative configurations.

If you run into any installation/configuration challenges, please let others know on the [slack channel](https://info201-a16.slack.com) so that others can anticipate the same issues.

## Git
`git` is a version control system that provides a set of commands that allow you to manage changes to written code, particularly when collaborating with other programmers (much more on this in [module 4](https://github.com/info201-w17/module4-git-basics)). For now, you'll need to [download](https://git-scm.com/downloads) and install the software. Note, if you are using a Windows machine, this will also install a program called Git Bash, which provides a text-based interface for executing commands on your computer. For alternative/additional Windows command-line tools, see below.

### GitHub
GitHub is a website that is used to store copies of code that are being managed with `git` (think "Imgur for code"). These learning modules are on GitHub (check out the URL!). You will also be using GitHub to turn in your programming assignments.

In order to use GitHub, you'll need to [create a free GitHub account](https://github.com/join), if you don't already have one. You should register a username that is identifiable as you (e.g., based on your name or your UW NetID). This will make it easier for us to collaborate and for the teaching staff to figure out who submitted what, rather than needing to figure out who 'LeetDesigner2099' is. This can be the start of a professional account you may use for the rest of your career!

## Command-line Tools (Bash)
The command-line provides a text-based interface for giving instructions to your computer (much more on this in [module 2](https://github.com/info201-w17/module2-command-line)). In this course, we'll largely use the command-line for navigating our computer's file structure, and executing commands that allow us to keep track of changes to the code we write (i.e., version control with `git`).

In order to use the command-line, you will need to use a **command shell** (a.k.a. a _command prompt_). This is a program that provides the interface to type commands into. In particular, we'll be working with the <a href="https://en.wikipedia.org/wiki/Bash_(Unix_shell)">Bash</a> shell, which provides a particular common set of commands common to Mac and Linux machines.

### Mac
On a Mac you'll want to use the built-in app called **Terminal**. You can open it by searching via Spotlight (hit Cmd (⌘) and Spacebar together, type in "terminal", then select the app to open it), or by finding it in the Applications/Utilities folder.

### Windows
On Windows, we recommend using [Git Bash](https://git-scm.com/downloads), which you should have installed along with `git` (above). Open this program to open the command-shell. This works great, since we'll primarily be using the command-line for performing version control.

- Note that Windows does come with its own command-prompt, called the _DOS Prompt_, but it has a different set of commands and features. _Powershell_ is a more powerful version of the DOS prompt if you really want to get into the Windows Management Framework. But Bash is more common in open-source programming like we'll be doing, and so we will be focusing on that set of commands.

Alternatively, the 64-bit Windows 10 Anniversary update (August 2016) _does_ include a beta version of an integrated Bash shell. You can access this by [enabling the subsystem for Linux](https://msdn.microsoft.com/en-us/commandline/wsl/install_guide) and then running `bash` in the command prompt. This is currently (Dec 2016) "beta" technology, but will suffice for our purposes if you can get it running.


## Text Editors
In order to write code, you need somewhere to write it (we don't want to write it in MS Word!). There are a variety of available programs that provide an interface for editing code. A major advantage of these programs is that they provide automatic formatting/coloring for easier interpretation of the code, along with cool features like auto-completion and integration with version control.

RStudio has a great built in text editor, but you'll sometimes want to use another text editor which is lighter weight (e.g., runs faster), more robust, or supports a different programming language. There are lots of different text editors out there, all of which have slightly different appearances and features. You only need to download and use one of the following programs (we recommend **Atom** as a default), but feel free to try out different ones to find something you like (and then evangelize about it to your friends!)

### Atom
[Atom](https://atom.io/) is a text editor built by the folks at GitHub and has been gaining in popularity. As an open source project, people are continually building (and making available) interesting/useful extensions. Its built-in spell-check is a great feature, especially for documents that require lots of written text. It also has excellent support for Markdown, a markup language we'll be using regularly in this course.

Click the "Download" button to download the installer `.exe` file, then double-click on that to install the application.

Once you've installed Atom, the trick to using it effectively is to get comfortable with the [Command Palette](http://flight-manual.atom.io/getting-started/sections/atom-basics/#command-palette). If you hit `Cmd+Shift+P`, Atom will open a small window where you can search for whatever you want the editor to do. For example, if you type in `markdown` you can get list of commands related to Markdown files (including the ability to open up a preview).

For more information about using Atom, see [the manual](http://flight-manual.atom.io/).

### Visual Studio Code
[Visual Studio Code](https://code.visualstudio.com/) (or VS Code; not to be confused with Visual Studio) is an open-source editor developed by Microsoft. While it focuses on web programming and JavaScript, it readily supports lots of languages including Markdown and R and provides a number of extensions for adding even more features. It has a similar command-palette to Atom, but isn't quite as nice for editing Markdown specifically. Although fairly new, it is updated regularly and has has become one of my main editors for programming.

### SublimeText
[SublimeText](https://www.sublimetext.com/3) is a very popular text editor with excellent defaults and a variety of available extensions (though you'll need to manage and install extensions to achieve the functionality offered by other editors out of the box). While the software can be used for free, every 20 or so saves it will prompt you to purchase the full version. This is my application of choice for when I just write to write a plain text file.

## RStudio
The primary programming language we will use throughout the course is R. It's a very powerful statistical programming language that is built to work well with large and diverse datasets. While you are able to execute R scripts without an interface, the RStudio interface provides a wonderful way to engage with the R language.

To install the RStudio program, select the **installer** for your operating system from the [downloads page](https://www.rstudio.com/products/rstudio/download/). Make sure to download the _free_ version scroll down to download a **free** version of RStudio:

![RStudio download selection](imgs/rstudio-download.png)

Once the download completes, double-click on the `.exe` file to run the installer. Simply follow the steps of the installer, and you should be prepared to use RStudio.

By downloading RStudio, you will also install the R programming language, if it is not already present in your operating system. However, if there are any problems with that you can also [install R separately](https://cran.rstudio.com/). Click on the download page for your operating system in order to find a link to the installer. On a Mac you're looking for the `.pkg` file, and for Windows you want to look in the `base` section (follow the link that to "install R for the first time").
