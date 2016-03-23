# Introduction to Unix Commands

### Steven Kneiser's notes for his [Spartan Hackers](http://spartanhackers.com/) talk

[![Bash Video](http://img.youtube.com/vi/UrMB1Pdwja0/0.jpg)](https://www.youtube.com/watch?v=UrMB1Pdwja0)

Windows users should download PuTTY:

```
http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html
```

## Getting Started (5 minutes)

- Why bash is important to know
- Understanding the directory structure (tree)

> Remember how, on your Desktop, you can manipulate files and folders?
>
> The entire filesystem for your computer is just a MASSIVE tree of folders and folders with files along the way.

Notable Directories
- Root "**/**" - The single folder at the core
- Home "**~**" - The folder containing everything for your user
- Working "**.**" - The current folder you're in

...also, I'm gonna refer to folders as directories here on out.

## Bits of Bash (20 minutes)

Got that shell open? Time for some basic navigation!

- **ls** - list directory contents
- **cd** - change working directory
- **touch** - change file access and modification times (creates a file)
- **rm** - remove directory entries
- **cp** - copy files
- **mv** - move files
- **clear** - clear the terminal screen

Now that you've got those under your belt, we need to talk about command options- or *flags*.  Flags are how we specify additional parameters to our commands similar to passing arguments to a function in programming.

For example: sure, **ls** lists directory contents but what if I want to see hidden dotfiles? I can include the **-a** option:

```shell
ls -a
```

Want a "long" listing with lots of additional system information?

```shell
ls -l
```

But how do we familiarize with all of these hidden options? *...I'm glad you asked.*

- **man** - format and display the on-line manual pages

# Time to wing it

Before we move on, you should copy this document onto your desktop:

```shell
curl --location goo.gl/NU44jC > ~/Desktop/unix.txt
```
This will prove a great resource for you to refer back to if you ever get lost or have any nagging questions after the workshop.

> I got you.  -Steven Kneiser

## My Mysterious & *Undisputably Dope* Project (10 minutes)

Finally! Time to do something both tangible *and dope*.  First thing we're gonna do is remote into a school server:

```shell
ssh your_net_id@arctic.cse.msu.edu
```

After entering your password you should be in your user's home directory (represented by the "**~**").  Next up, we're gonna make a directory for this project called "**web**" and hop right in there:

```shell
mkdir web
cd web
```

This seems like the PERFECT place to dump my mysterious & *undisputably dope* file:

```shell
curl --location goo.gl/W5GHZd > index.html
```

*Rubs hands together with a devilish grin*

Now before I give anything away, I want you to run these two commands:

```shell
chmod -R a+rX ~/web
chmod 701 ~/
```

**Congratulations**, you've officially setup your very own student homepage! Don't believe me? Visit:

```
cse.msu.edu/~your_net_id
```

## Q&A & Unix Tips (25 minutes)

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
- package-management

#### Advanced Miscellaneous

- keyboard shortcuts (reverse-i search)
- curly brace completion
- bash scripting
- crontab

## Further reading

#### [*This Repo*](https://github.com/theshteves/bash-workshop)

#### Other Unix tutorials

- [CSE-320 Bash reference **READ THIS IF NOTHING ELSE**](http://www.ee.surrey.ac.uk/Teaching/Unix/)
- [A curated list of awesome command-line guides, frameworks, etc](https://github.com/alebcay/awesome-shell)
- [Advancing in the Bash Shell](http://samrowe.com/wordpress/advancing-in-the-bash-shell/)
- [Advanced Bash-Scripting Guide: An in-depth exploration of the art of shell scripting](http://www.tldp.org/LDP/abs/html/)

#### Other shells

- [Z Shell (zsh) tutorial](http://reasoniamhere.com/2014/01/11/outrageously-useful-tips-to-master-your-z-shell/)
- [Great resource for customizing your zsh](https://github.com/robbyrussell/oh-my-zsh)

#### More on Unix:

- [Wikipedia - Unix](https://en.wikipedia.org/wiki/Unix)
- [dotJS Talk w/ some historical background knowledge](https://www.youtube.com/watch?v=UIDb6VBO9os)

#### Learning Vim?

- [My favorite cheatsheet](http://i.imgur.com/YLInLlY.png)
- [Learn from others' screencasts](http://vimcasts.org/)
- [Advanced vim registers](http://blog.sanctum.geek.nz/advanced-vim-registers/)

#### Miscellaneous

- [Jealous of my colorful bash prompt? Generate a dope one](https://www.kirsle.net/wizards/ps1.html)
- [An even more beautiful prompt](https://github.com/milkbikis/powerline-shell) recommended by [@nicovergara](https://github.com/nicoevergara)
- [Scheduling routine tasks on your crontab](http://kvz.io/blog/2007/07/29/schedule-tasks-on-linux-using-crontab/)
- [Passing command-line arguments to python](https://docs.python.org/3/library/argparse.html)
