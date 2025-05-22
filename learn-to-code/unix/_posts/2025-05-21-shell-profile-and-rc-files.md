---
layout: post
author: brittni watkins
date: 2025-05-21 12:00:00 -0000
modified_date: 2025-05-21
title: "shell profile and rc files"
excerpt: "When a Unix shell is initialized, it reads and executes commands from a set of configuration files. These files are used to set up the shell environment, including environment variables, aliases, and functions."
tags:
  - unix
  - command line
  - shell
  - bash
  - z shell
  - profile file
  - rc file
  - configuration
  - environment variables
---

When a Unix shell is initialized, it reads and executes commands from a set of configuration files. These files are used to set up the shell environment, including environment variables, aliases, and functions. The specific files that are executed depend on the type of shell being used and whether the shell has registered a login operation.

----

## table of contents

[the home directory](#the-home-directory)

[shell profile files](#shell-profile-files)

[shell rc files](#shell-rc-files)

[editing profile and rc files](#editing-profile-and-rc-files)
- [editing on macOS](#editing-on-macos)
- [editing on Windows](#editing-on-windows)
- [editing from the command line](#editing-from-the-command-line)

[resources and references](#resources-and-references)

----

## the home directory

Profile files and RC files should be located in the user's home directory. To see the location of your home directory, execute one of the following commands in your preferred Unix shell.

```shell
echo $HOME
```

```shell
cd ~
pwd
```

If a profile file or RC file does not exist, you can create it using the `touch` command. For example, to create a `.bash_profile` file, execute the following command in your preferred Unix shell.

```shell
touch ~/.bash_profile
```

Additional information about Unix shell commands can be found in the [useful unix commands guide]({% post_url learn-to-code/unix/2025-05-14-useful-unix-commands %}).

----

## shell profile files

Shell profile files are executed when a user logs in to the shell. On a personal computer, opening a new shell window will typically register as a login operation.

In [Bash shell](https://en.wikipedia.org/wiki/Bash_(Unix_shell)), the profile file is typically called `.bash_profile`.

In [Z shell](https://en.wikipedia.org/wiki/Z_shell), the profile file is typically called `.zprofile`.

----

## shell rc files

RC files are executed when a new shell is started or initialized. This includes opening a new shell window or executing a shell script.

In [Bash shell](https://en.wikipedia.org/wiki/Bash_(Unix_shell)), the RC file is typically called `.bashrc`.

In [Z shell](https://en.wikipedia.org/wiki/Z_shell), the profile file is typically called `.zshrc`.

----

## editing profile and rc files

### editing on macOS

You can edit profile and RC files on macOS using the `TextEdit` application. You can open files in `TextEdit` from the command line using the `open` command. For example, to open the `.bashrc` file, execute the following command in your preferred Unix shell.

```shell
open ~/.bashrc
```

### editing on Windows

You can edit profile and RC files on Windows using the `Notepad` application. You can open files in `Notepad` from the command line using the `explorer` command. For example, to open the `.bashrc` file, execute the following command in your preferred Unix shell.

```shell
explorer ~/.bashrc
```

### editing from the command line

You can edit profile and RC files directly from the command line using a wide range of command line text editors, including [`nano`](https://www.nano-editor.org/), [`vi`](https://en.wikipedia.org/wiki/Vi_(text_editor)), and [`vim`](https://www.vim.org/).

*A guide on editing files in vi is coming soon!*

<!-- TODO - link to editing files in vi post -->

----

## resources and references

[Wikipedia - Bash (Unix shell)](https://en.wikipedia.org/wiki/Bash_(Unix_shell))

[Wikipedia - Z shell](https://en.wikipedia.org/wiki/Z_shell)

[nano](https://www.nano-editor.org/)

[Wikipedia - GNU nano](https://en.wikipedia.org/wiki/GNU_nano)

[Wikipedia - vi (text editor)](https://en.wikipedia.org/wiki/Vi_(text_editor))

[vim](https://www.vim.org/)

[Wikipedia - Vim (text editor)](https://en.wikipedia.org/wiki/Vim_(text_editor))
