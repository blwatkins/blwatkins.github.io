---
layout: post
author: brittni watkins
date: 2025-05-14 22:00:00 -0000
title: "absolute and relative paths"
excerpt: "When specifying the location of files and folders on a computer system, it is important to know the difference between a relative path and an absolute path, and which is most appropriate for your code."
tags:
  - paths
  - absolute paths
  - relative paths
  - unix
  - bash
  - z shell
---

When specifying the location of files and folders on a computer system, it is important to know the difference between a relative path and an absolute path, and which is most appropriate for your code.

----

## table of contents

- [absolute path](#absolute-path)
- [relative path](#relative-path)
- [paths with spaces](#paths-with-spaces)

----

## absolute path

An absolute path is the path to a file or directory from the root of the computer.

On Unix-like systems, absolute paths begin with `/` (e.g. `/Users/username/`).

On Windows systems, absolute paths begin with the drive name (e.g. `C:/Users/username/`).

In a Unix shell, you print the absolute path of your working directory with the `pwd` command. Additional information about Unix shell commands can be found in the [useful unix commands guide]({% post_url learn-to-code/unix/2025-05-14-useful-unix-commands %}).

I rarely recommend using absolute paths in any situation.  The absolute path to a file on one machine will likely be very different from the path to the file on a different machine, which could lead to errors, crashes, and unexpected behaviors in your program.

----

## relative path

A relative path allows us to reference the location of a file or directory relative to the working directory.

Certain characters in relative paths can be use to indicate different directories relative to the working directory.

`..` is used to indicate the directory one level up from the working directory.

`.` is used to indicate the working directory.

`~` is used to indicate your `$HOME` directory.

If you do not know the location of your home directory, you can print it using the `echo` command in a Unix shell.

```shell
echo $HOME
```

Additional information about Unix shell commands can be found in the [useful unix commands guide]({% post_url learn-to-code/unix/2025-05-14-useful-unix-commands %}).

### `cd` with relative paths

In a Unix shell, you can use the `cd` command to change your working directory. Let's say we have three directories: <span style="color: red;">Level-0</span>/<span style="color: blue;">Level-1</span>/<span style="color: green;">Level-2</span>.

From <span style="color: red;">Level-0</span>, `cd Level-1` will take you to <span style="color: blue;">Level-1</span>.

From <span style="color: blue;">Level-1</span>, `cd ..` will take you to <span style="color: red;">Level-0</span>.

From <span style="color: blue;">Level-1</span>, `cd ./Level-2` will take you to <span style="color: green;">Level-2</span>.

From <span style="color: green;">Level-2</span>, `cd ../..` will take you to <span style="color: red;">Level-0</span>.

From <span style="color: red;">Level-0</span>, `cd Level-1/Level-2` will take you to <span style="color: green;">Level-2</span>.

From <span style="color: blue;">Level-1</span>, `cd .././Level-1/Level-2/..` will take you to <span style="color: blue;">Level-1</span>.

Additional information about Unix shell commands can be found in the [useful unix commands guide]({% post_url learn-to-code/unix/2025-05-14-useful-unix-commands %}).

----

## paths with spaces

When executing commands in a Unix shell, if any folder in a directory path has a space character in its name, the path must be surrounded by quotes.

```shell
cd '../directory with spaces/sub-1'

ls './directory with spaces'

mkdir 'directory with spaces'
```

Additional information about Unix shell commands can be found in the [useful unix commands guide]({% post_url learn-to-code/unix/2025-05-14-useful-unix-commands %}).

----

This tutorial was last updated on Thursday, May 15, 2025.
