---
layout: post
author: brittni watkins
date: 2025-05-14 16:00:00 -0000
modified_date: 2025-05-20
title: "useful unix commands"
excerpt: "This tutorial will walk you through some Unix shell commands that will be useful to know as you progress on your coding journey."
tags:
  - unix
  - commands
  - command line
  - shell
  - bash
  - z shell
---

A Unix shell provides a text-based user interface for Unix-like operating systems. The shell is both an interactive command language and a scripting language, and it is used by the operating system to control the execution of the system using shell scripts.

This tutorial will walk you through some Unix shell commands that will be useful to know as you progress on your coding journey. This guide is not an exhaustive list.

----

## table of contents

[how to execute a unix shell command](#how-to-execute-a-unix-shell-command)

[unix shell shortcuts](#unix-shell-shortcuts)

[commands](#commands)
- [`pwd`](#print-working-directory)
- [`whoami`](#print-your-username)
- [`date`](#print-the-current-date-and-time)
- [`echo`](#print-something)
- [`clear`](#clear-the-shell-window)
- [`ls`](#list-the-directory-contents)
- [`cd`](#change-the-working-directory)
- [`touch`](#create-a-file)
- [`mkdir`](#create-a-directory-folder)
- [`chmod`](#change-file-permissions)
- [`export`](#set-the-value-of-an-environment-variable)
- [`which`](#print-the-path-of-this-command)
- [`where` / `which -a`](#print-all-paths-to-this-command)
- [`bash`](#start-a-bash-shell-instance)
- [`zsh`](#start-a-z-shell-instance)
- [`exit`](#exit-the-current-shell-instance)

[resources and references](#resources-and-references)

----

## how to execute a unix shell command

A Unix shell command can be executed through a CLI application running a Unix shell instance, or it can be executed as part of a Unix shell script.

Additional information about CLI applications can be found in the [software for unix guide]({% post_url learn-to-code/unix/2025-05-21-software-for-unix %}).

Once you have opened the CLI application, type the command and press `ENTER` or `RETURN` to execute it. Some commands will print text as a part of their execution, and some will not. An error message will usually be printed if something has gone wrong during the program execution or if the command and its arguments were not structured properly.

*A guide on how to create and run a Unix shell script is coming soon!*

<!-- TODO - link to creating and running a shell script post -->

----

## unix shell shortcuts

Use the `TAB` key to autocomplete file, directory, and command names.

Use the `UP` arrow key to scroll through previous commands.

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

### print something

```shell
echo STRING_HERE
```

The `echo` command will print the given string.

> [!TIP]
> Fun fact: Want to make your computer beep? Try the following: 
> `echo -e "\a"`

```shell
echo $VARIABLE_NAME_HERE
```

When given an environment variable name, such as `$HOME` or `$PATH`, the `echo` command will print the value of the given variable.

#### examples

```shell
echo "Hello, World!"
echo $HOME
```

### clear the shell window

```shell
clear
```

The `clear` command will clear the shell window.

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

### change the working directory

```shell
cd DIRECTORY_PATH_HERE
```

The `cd` command will change the working directory to the directory with the given absolute or relative path.

Additional information about paths can be found in the [absolute and relative paths guide]({% post_url learn-to-code/unix/2025-05-14-absolute-and-relative-paths %}).

### create a file

```shell
touch FILENAME_HERE
```

The `touch` command creates a file.

```shell
touch FILE_PATH_HERE
```

When executing the `touch` command, the filename argument can also be a relative or absolute path to the file you are creating.

Additional information about paths can be found in the [absolute and relative paths guide]({% post_url learn-to-code/unix/2025-05-14-absolute-and-relative-paths %}).

#### examples

```shell
touch my-text-file.txt
touch ./my-directory/MyJavaClass.java
```

### create a directory (folder)

```shell
mkdir DIRECTORY_PATH_HERE
```

The `mkdir` command creates a folder, also known as a directory. The directory path argument can be an absolute path or a relative path.

Additional information about paths can be found in the [absolute and relative paths guide]({% post_url learn-to-code/unix/2025-05-14-absolute-and-relative-paths %}).

### change file permissions

```shell
chmod PERMISSIONS_HERE FILE_PATH_HERE
```

The `chmod` command updates the permissions of the given file using the given permissions.

Permissions can be provided in symbolic mode or octal mode.

*A guide on file permissions is coming soon!*

<!-- TODO - link to file permissions post -->

#### examples

```shell
touch my-text-file.txt
chmod 444 my-text-file.txt
chmod ugo+w my-text-file.txt
```

### set the value of an environment variable

```shell
export VARIABLE_NAME_HERE=VARIABLE_VALUE_HERE
```

The `export` command will set the given variable to the given value. When executed in a Unix shell, this change will only be active for the current shell session.

If an environment variable needs to have some value in every shell session, it is recommended to set that variable in the appropriate shell profile file or shell RC file.

*A guide on shell profile and RC files is coming soon!*

<!-- TODO - link to shell profile and rc files post -->

To confirm the variable has been set properly, you can print its value using the [`echo`](#print-something) command.

```shell
echo $VARIABLE_NAME_HERE
```

#### examples

```shell
export SOME_VARIABLE="some value"
echo $SOME_VARIABLE
```

### print the path of this command

```shell
which COMMAND_NAME_HERE
```

The `which` command prints the absolute path to the location of the given command, provided as an argument.

#### examples

```shell
which ruby
which python
```

### print all paths to this command

```shell
where COMMAND_NAME_HERE
```

```shell
which -a COMMAND_NAME_HERE
```

The `where` command and the `which -a` command are equivalent; they both print all paths that could be used to execute the given command.

The `where` command gives you all locations of the given program; the `which` command tells you which one will be used when you execute that program.

#### examples

```shell
where ruby
which -a ruby
```

### start a Bash shell instance

```shell
bash
```

The `bash` command will start a run of the Bash shell inside the current shell instance.

### start a Z shell instance

```shell
zsh
```

The `zsh` command will start a run of the Z shell inside of the current shell instance.

### exit the current shell instance

```shell
exit
```

The `exit` command can be used to exit the current shell instance.

----

## resources and references

[AWS - What is a CLI?](https://aws.amazon.com/what-is/cli/)

[Wikipedia - Unix shell](https://en.wikipedia.org/wiki/Unix_shell)

[Wikipedia - Bash (Unix shell)](https://en.wikipedia.org/wiki/Bash_(Unix_shell))

[Wikipedia - Z shell](https://en.wikipedia.org/wiki/Z_shell)

[explainshell](https://explainshell.com/)

[MULTACOM: Understanding File Permissions](https://www.multacom.com/faq/password_protection/file_permissions.htm)
