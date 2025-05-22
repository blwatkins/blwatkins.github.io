---
layout: post
author: brittni watkins
date: 2025-05-22 01:00:00 -0000
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

Profile files and RC files should be located in the user's home directory. To see the location of your home directory, execute one of the following commands in your preferred Unix shell.

```shell
echo $HOME
```

```shell
cd ~
pwd
```

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

## resources and references

[Wikipedia - Bash (Unix shell)](https://en.wikipedia.org/wiki/Bash_(Unix_shell))

[Wikipedia - Z shell](https://en.wikipedia.org/wiki/Z_shell)
