# Tutorial 1 - The Command Line/Unix

On the more popular operating systems like Windows or Mac, we typically use our mouse or trackpad to click on icons to access files and applications. However, there are many other ways for us to communicate with our computers. The command line is a text-based interface that is quick, powerful and straight-to-the-point. It allows users to communicate with their computers or files directly. In other words, you can navigate to, open and modify files and folders on your computer without your mouse!

Unix is an operating system (similar to Windows or Mac OSX). It's made up of three parts: the <i>kernel</i>, the <i>shell</i> and the <i>programs</i>. 

#### If you're curious to know:

`kernel` - operating system hub which allocates time and memory to programs; handles file storage and system calls

`shell` - the interface between the user and the kernel; the command line interpreter (CLI) which interprets the user's commands and carries them out

`programs` - commands

## Getting Started
### Accessing a Unix-based OS
Download [Ubuntu for your Desktop](https://ubuntu.com/download/desktop).

Lost? Here's an excellent tutorial which guides Windows 10 users on Ubuntu installation:
[![How to Install Ubuntu 20.04 LTS on VirtualBox in Windows 10](http://img.youtube.com/vi/x5MhydijWmc/0.jpg)](https://www.youtube.com/watch?v=x5MhydijWmc)

When you have successfully installed and run Ubuntu on your computer, search for and open up the `Terminal`.

## Basic Commands
When you open the terminal, you start in your home directory by default. Your home directory may have the same name as your computer's username. This is where your files and folders are saved.

In the terminal, type:
```bash
pwd
```
This <i>prints your working directory</i>, or the directory that you are in presently. 

### Listing Files and Folders
`ls` lists the contents of your current working directory. 
To find out what is in your home directory, type:
```bash
ls
```
Hidden files begin with a dot (.) and usually contain important program configuation information. Don't change these contents unless you absolutely must! To view these hidden files, type the command with an option:
```
ls -a
```
`options` change the behaviour of a command.


### Making Directories


`cd` To navigate to your home folder by default, type
```bash
cd
```


## Resources
* [Codecademy](https://www.codecademy.com/catalog/language/bash)
* [LabEx - Prctice Linux Commands](https://labex.io/courses/linux-basic-commands-practice-online)
* [Unix Tutorial for Beginners](http://www.ee.surrey.ac.uk/Teaching/Unix/)
