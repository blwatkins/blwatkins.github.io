---
layout: post
author: brittni watkins
date: 2025-05-14 15:35:00 -0000
title: "useful unix commands"
excerpt: "This tutorial will walk you through some Unix shell commands that will be useful to know as you progress on your coding journey."
tags:
  - unix
  - commands
  - bash
  - z shell
---

A command line interface (CLI) is a text-based interface where you can input commands that interact with a computer’s operating system. A Unix shell provides a command line user interface for Unix-like operating systems.  The shell is both an interactive command language and a scripting language, and is used by the operating sustem to control the execution of the system using shell scripts.

There are many Unix shell programs available to developers, including [Bash](https://en.wikipedia.org/wiki/Bash_(Unix_shell)) and [Z shell](https://en.wikipedia.org/wiki/Z_shell).

To access a Unix shell on a Windows machine, [follow these steps to install Git and GitBash]({% post_url learn-to-code/version-control/git/2025-05-13-how-to-install-git %}). GitBash will be your Unix shell CLI application.

To access a Unix shell on a macOS machine, open the Terminal application. You can find the Terminal application in your `Applications` folder on your computer or by searching for "Terminal" in the Spotlight Search.

This tutorial will walk you through some Unix shell commands that will be useful to know as you progress on your coding journey. This guide is not an exhaustive list.

----

## table of contents

- [`pwd`](#print-working-directory)
- [`whoami`](#print-your-username)
- [`ls`](#list-the-directory-contents)

----

## Commands

### print working directory

```shell
pwd
```

This command prints the absolute file path of your current location in the shell. Your current location will correspond to some folder in your computer's file system.

### print your username

```shell
whoami
```

This command prints your username. This can be useful to check your username when you are connected to a remote server.

### list the directory contents

```shell
ls
```

This command prints all the visible files and folders in our working directory.

```shell
ls -l
```

When we add the `-l` flag to the `ls` command, the visible files and folders will be printed in a long list format.

```shell
ls -a
```

When we add the `-a` flag to the `ls` command, the command will list all the files and folders in our working directory, including hidden files and folders.

Hidden files and folders will always have a name that begins with `.` (e.g. `.bash_profile`).

----

## resources and references

[AWS - What is a CLI?](https://aws.amazon.com/what-is/cli/)

[Wikipedia - Unix shell](https://en.wikipedia.org/wiki/Unix_shell)

[Wikipedia - Bash (Unix shell)](https://en.wikipedia.org/wiki/Bash_(Unix_shell))

[Wikipedia - Z shell](https://en.wikipedia.org/wiki/Z_shell)

[explainshell](https://explainshell.com/)

----

This tutorial was last updated on Wednesday, May 14, 2025.
