---
layout: post
author: brittni watkins
date: 2025-05-14 16:00:00 -0000
title: "useful unix commands"
excerpt: "This tutorial will walk you through some Unix shell commands that will be useful to know as you progress on your coding journey."
tags:
  - unix
  - commands
  - bash
  - z shell
---

A command line interface (CLI) is a text-based interface where you can input commands that interact with a computer’s operating system. A Unix shell provides a command line user interface for Unix-like operating systems.  The shell is both an interactive command language and a scripting language, and is used by the operating sustem to control the execution of the system using shell scripts.

This tutorial will walk you through some Unix shell commands that will be useful to know as you progress on your coding journey. This guide is not an exhaustive list.

----

## table of contents

[how to execute a unix shell command](#how-to-execute-a-unix-shell-command)

[unix shell shortcuts](#unix-shell-shortcuts)

[commands](#commands)
- [`pwd`](#print-working-directory)
- [`whoami`](#print-your-username)
- [`date`](#print-the-current-date-and-time)
- [`ls`](#list-the-directory-contents)
- [`clear`](#clear-the-shell-window)
- [`cd`](#change-the-working-directory)
- [`which`](#print-the-path-of-this-command)

----

## how to execute a unix shell command

A Unix shell command can be executed through a CLI application running a Unix shell instance, or it can be executed as part of a Unix shell script.

There are many Unix shell programs available to developers, including [Bash](https://en.wikipedia.org/wiki/Bash_(Unix_shell)) and [Z shell](https://en.wikipedia.org/wiki/Z_shell). To access a Unix shell on a Windows machine, [follow these steps to install Git and GitBash]({% post_url learn-to-code/version-control/git/2025-05-13-how-to-install-git %}). GitBash will be your Unix shell application. To access a Unix shell on a macOS machine, open the Terminal application. You can find the Terminal application in your `Applications` folder on your computer or by searching for "Terminal" in the Spotlight Search.

Once you have opened the CLI application, type the command and press `ENTER` or `RETURN` to execute it. Some commands will print text as a part of their execution, and some will not. An error message will usually be printed if something has gone wrong during the program execution or if the command and its arguments were not structured properly.

*A guide on how to create and run a Unix shell script is coming soon!*

----

## unix shell shortcuts

Use the `TAB` key to autocomplete file, directory, and command names.

Use the `UP` arrrow key to scroll through previous commands.

Use the `DOWN` arrow key to scroll forward through previous commands.

----

## commands

### print working directory

```shell
pwd
```

The `pwd` command prints the absolute file path of your current location in the shell. Your current location will correspond to some folder in your computer's file system.

### print your username

```shell
whoami
```

The `whoami` command prints your username. This can be useful to check your username when you are connected to a remote server.

### print the current date and time

```shell
date
```

The `date` command prints the current date and time.

### list the directory contents

```shell
ls
```

The `ls` command prints all the visible files and folders in our working directory.

```shell
ls -l
```

When we add the `-l` flag to the `ls` command, the visible files and folders will be printed in a long list format.

```shell
ls -a
```

When we add the `-a` flag to the `ls` command, the command will list all the files and folders in our working directory, including hidden files and folders.

Hidden files and folders will always have a name that begins with `.` (e.g. `.bash_profile`).

```shell
ls -al
```

When we add both the `-a` and `-l` flags to the `ls` command, the command will list all files in our working directory, including hidden files, in a long list format.

```shell
ls DIRECTORY_PATH_HERE
```

We can use the `ls` command to print the contents of a different directory by providing the absolute or relative path to the directory.

Additional information about paths can be found in the [absolute and relative paths guide]({% post_url learn-to-code/unix/2025-05-14-absolute-and-relative-paths %}).

### clear the shell window

```shell
clear
```

The `clear` command will clear the shell window.

### change the working directory

```shell
cd DIRECTORY_PATH_HERE
```

The `cd` command will change the working directory to the directory with the given absolute or relative path.

Additional information about paths can be found in the [absolute and relative paths guide]({% post_url learn-to-code/unix/2025-05-14-absolute-and-relative-paths %}).

### print the path of this command

```shell
which COMMAND_NAME_HERE
```

The `which` command prints the absolute path to the location of the given command, provided as an argument.

```shell
which ruby
```

----

## resources and references

[AWS - What is a CLI?](https://aws.amazon.com/what-is/cli/)

[Wikipedia - Unix shell](https://en.wikipedia.org/wiki/Unix_shell)

[Wikipedia - Bash (Unix shell)](https://en.wikipedia.org/wiki/Bash_(Unix_shell))

[Wikipedia - Z shell](https://en.wikipedia.org/wiki/Z_shell)

[explainshell](https://explainshell.com/)

----

This tutorial was last updated on Tuesday, May 20, 2025.
