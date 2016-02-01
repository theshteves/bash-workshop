# Introduction to Unix Commands

### Steven Kneiser's notes for his [Spartan Hackers](http://spartanhackers.com/) talk

##### Description:

> What's behind that hacker-green terminal, you ask?
> Our VP Steven Kneiser knows  ...and YOU WILL TOO!
> That's right.  Fresh off his impromptu "Surviving your first Hackathon", 
> Steven is rebounding with the most high-energy & unassuming talk of the semester.
>
> DON'T MISS this absurdly over-prepared workshop bundled with technical breakdowns from a > (yet to be announced) Startup Founder in the Lansing area.
> Not you first-time?  Thought you were ahead of the curve?  ...think again.
>
> Their goal? To get you comfortable & employer-ready with the command line in. 1. HOUR.
> Professors WILL ASSUME you already know this.
> Bring your chargers and empty stomachs while Steven tricks you into an invaluable skillset.

## BEGINNER-LEVEL (15 minutes)

#### General Overview (For people to setup and get ready)

- mention structure of talk to prep people for when they should really be attentive
- super-brief history ??? (see matt & yoseph's readings)
- there are a couple popular shells (esp. zsh) but we'll be sticking to bash because it's more primitive and most of zsh aims to just simplify & improve upon it

If computers are simply 0s and 1s, and code is how we manipulate those bits, but we are used to code in a restricted console window.  This is portal for you to talk directly to your computer, similar to the way an application is designed to talk directly to the user.   

You're probably gonna spend more time simply moving things around and accessing files than writing scripts that give you new functionality.  Working with the command line is a really competent way to work.  It's working further under the hood and what you learn about working at this level that will greatly inform your development process later on as a software engineer.  

- Using the text-based command line is just using your computer, ...without the graphics.
- Directory Structure (tree)

Remember how, on your Desktop, you can manipulate files and folders?
The entire filesystem for your computer is just a MASSIVE tree of folders and folders with files along the way.
The two notable directories then, are the root directory (at the very top)
...and your home directory which quite literally holds (your desktop folder (yes, it is folder), as well as your downloads, documents, etc).

- your home directory is gonna be your DEFAULT directory (I'm gonna reffer to folders as directoriess here on out) 

#### Basic Navigation

- ls & cd
- touch & rm
- cp & mv
- mkdir & rmdir
- cat & editors
- understanding flags
- finding help (man, apropos, ...then google)
- tab-completion

#### Bash Redirection & Search

- piping 
- (less & more)?
- grep
- sort & awk & wc  
- find

## INTERMEDIATE-LEVEL (35 minutes)

#### Filesystem security

- reading access rights
- chmod
- sudo & su

#### Running processes (language-specific consoles etc)

- ps
- sending signals
- jobs (listing and suspending)
- fg & bg

#### Customizing your environment (dotfiles)

- environmental variables (echo & printenv)
- .bash_profile & rc's (SHELL-DEPENDENT)
- aliases & functions
- SSH & simplifying (.ssh/config)

## "ADVANCED"-LEVEL (10 minutes)

- keyboard shortcuts (reverse-i search)
- curly brace completion
- bash scripting
- crontab

#### Sysadmin basics?

- package-management
- user-management

# Further reading

- this repo
- other thorough UNIX tutorials
- other shells (zsh & oh-my-zsh)
- Unix history
