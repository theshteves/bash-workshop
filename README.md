# Introduction to Unix Commands

### Steven Kneiser's notes for his [Spartan Hackers](http://spartanhackers.com/) talk

Windows users should download PuTTY:

```
http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html
```

#### Getting Started



#### Bits of Bash

Copy this document onto your desktop:

```shell
curl --location goo.gl/NU44jC > unix.txt
```

# Project



# Tips & Q&A








## BEGINNER-LEVEL (15 minutes)

#### General Overview (For people to setup and get ready)

- mention structure of talk to prep people for when they should really be attentive
- super-brief history ??? (see matt & yoseph's readings)
- there are a couple popular shells (esp. zsh) but we'll be sticking to bash because it's more primitive and most of zsh aims to just simplify & improve upon it

We think of computers are simply 0s and 1s, and code is how we manipulate those bits, but we are used to code in a restricted console window.  This is portal for you to talk directly to your computer, similar to the way an application is designed to talk directly to the user.   

You're probably gonna spend more time simply moving things around and accessing files than writing scripts that give you new functionality.  Working with the command line is a really competent way to work.  It's working further under the hood and what you learn about working at this level that will greatly inform your development process later on as a software engineer.  

- Using the text-based command line is just using your computer, ...without the graphics.
- Directory Structure (tree)

Remember how, on your Desktop, you can manipulate files and folders?
The entire filesystem for your computer is just a MASSIVE tree of folders and folders with files along the way.
The two notable directories then, are the root directory (at the very top)
...and your home directory which quite literally holds your desktop folder (yes, it is folder), as well as your downloads, documents, etc.

- your home directory is gonna be your DEFAULT directory (I'm gonna refer to folders as directoriess here on out) 

#### Basic Navigation

- ls & cd
- touch & rm
- cp & mv
- mkdir & rmdir
- cat & editors (nano, vim, emacs)
- understanding flags
- *tab-completion & clear*
- **finding help (man, apropos, ...then google)**

#### Bash Redirection & Search

- piping 
- less/more & head & tail
- grep
- sort & awk & wc  
- find

## INTERMEDIATE-LEVEL (35 minutes)

#### Filesystem security

- reading access rights
- chmod
- sudo & su

#### Running processes (language-specific consoles etc)

- jobs (listing and suspending)
- fg & bg
- ps
- sending signals

#### Customizing your environment (dotfiles)

- environmental variables (echo & printenv)
- **.profile's & rc's (SHELL-DEPENDENT)**
- aliases & functions
- SSH & simplifying (.ssh/config)

## "ADVANCED"-LEVEL (10 minutes)

- keyboard shortcuts (reverse-i search)
- curly brace completion
- bash scripting
- crontab

#### *Sysadmin basics?*

- package-management
- user-management

# Further reading

#### [*This Repo*](https://github.com/theshteves/bash-workshop)

#### Other Unix tutorials

- [CSE-320 Bash reference](http://www.ee.surrey.ac.uk/Teaching/Unix/)
- [Advancing in the Bash Shell](http://samrowe.com/wordpress/advancing-in-the-bash-shell/)
- [Advanced Bash-Scripting Guide: An in-depth exploration of the art of shell scripting](http://www.tldp.org/LDP/abs/html/)

#### Other shells

- [A curated list of awesome command-line guides, frameworks, etc](https://github.com/alebcay/awesome-shell)
- [Great resource for customizing your zsh](https://github.com/robbyrussell/oh-my-zsh)
- [Z Shell (zsh) tutorial](http://reasoniamhere.com/2014/01/11/outrageously-useful-tips-to-master-your-z-shell/)

#### More on Unix:

- [Wikipedia - Unix](https://en.wikipedia.org/wiki/Unix)
- [dotJS Talk w/ some historical background knowledge](https://www.youtube.com/watch?v=UIDb6VBO9os)

#### Miscellaneous

- [Python: Working with bash](https://docs.python.org/3/library/argparse.html)

