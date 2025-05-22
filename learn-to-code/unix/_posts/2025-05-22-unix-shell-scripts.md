---
layout: post
author: brittni watkins
date: 2025-05-22 12:00:00 -0000
modified_date: 2025-05-22
title: "unix shell scripts"
excerpt: "This guide will cover the basics of creating, writing, and executing shell scripts in Unix-like operating systems."
tags:
  - unix
  - shell scripts
  - command line
  - shell
  - bash
  - z shell
---

A shell script is a program designed to be run by a Unix shell. Applications of shell scripts include automating tasks and batching Unix operations.

This guide will cover the basics of creating, writing, and executing shell scripts in Unix-like operating systems.

----

## table of contents

[creating a shell script file](#creating-a-shell-script-file)

[opening a shell script file](#opening-a-shell-script-file)

[writing a shell script](#writing-a-shell-script)
- [shebang](#shebang)
- [comments](#comments)
- [variables](#variables)
- [functions](#functions)
- [conditionals](#conditionals)
- [loops](#loops)
- [command line arguments](#command-line-arguments)

[resources and references](#resources-and-references)

----

## creating a shell script file

A shell script file can be created using any text editor. A list of popular text editors can be found in the [text editors guide](TODO). If you would like to create a shell script file using the command line, you can use the `touch` command to create an empty file. For example, to create a shell script file named `my-script.sh`, you would execute the following command in the terminal.

```shell
touch my-script.sh
```

Additional information about unix shell commands can be found in the [unix commands guide](TODO).

The extension of your shell script file will vary depending on the shell you plan to execute it with and your personal preferences. Most shell scripts use the `.sh` extension, for example `my-script.sh`. If you are using the Bash shell, you can also use the `.bash` extension, for example `my-script.bash`. If you are using the Z shell, you can use the `.zsh` extension, for example `my-script.zsh`. You could also have a shell script file with no extension at all, for example `my-script`.

----

## opening a shell script file

----

## writing a shell script

### shebang

The first line of any shell script file should be the shebang line. The shebang line tells the operating system which Unix shell interpreter to use to execute the script. The shebang line starts with `#!` followed by the path to the interpreter. For example, if you are using the Bash shell, the shebang line would look like this:

```bash
#!/bin/bash
```
If you are using the Z shell, the shebang line would look like this:

```zsh
#!/bin/zsh
```

### comments

Comments in a shell script start with the `#` symbol. Comments are ignored by the shell interpreter.

```shell
# this is a comment
pwd
```

### variables

More information about variables is coming soon!

<!-- TODO - complete variables in shell scripts section -->

### functions

More information about functions is coming soon!

<!-- TODO - complete functions in shell scripts section -->

### conditionals

More information about conditionals is coming soon!

<!-- TODO - complete conditionals in shell scripts section -->

### loops

More information about loops is coming soon!

<!-- TODO - complete loops in shell scripts section -->

### command line arguments

More information about command line arguments is coming soon!

<!-- TODO - complete command line arguments in shell scripts section -->

----

## resources and references

[Baeldung: How to Use Command Line Arguments in a Bash Script](https://www.baeldung.com/linux/use-command-line-arguments-in-bash-script)

[Red Hat: Adding arguments and options to your Bash scripts](https://www.redhat.com/sysadmin/arguments-options-bash-scripts)
