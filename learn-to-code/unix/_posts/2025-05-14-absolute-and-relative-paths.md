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

## absolute path

An absolute path is the path to a file or directory from the root of the computer.

On Unix-like systems, absolute paths begin with `/` (e.g. `/Users/username/`).

On Windows systems, absolute paths begin with the drive name (e.g. `C:/Users/username/`).

In a Unix shell CLI (command line interface), you print the absolute path of your working directory with the `pwd` command.

I rarely recommend using absolute paths in any situation.  The absolute path to a file on one machine will likely be very different from the path on a different machine, which could lead to errors, crashes, and unexpected behaviors in your program.

## relative path

A relative path allows us to reference the location of a file or directory relative to the working directory.

Certain characters in relative paths can be use to indicate different directories relative to the working directory.

`..` is used to indicate the directory one level up from your current location.

`.` is used to indicate the directory you are currently located in.

`~` is used to indicate your `$HOME` directory.

If you do not know the location of your home directory, you can print it using the `echo` command in a Unix shell CLI.

```shell
echo $HOME
```

### `cd` with relative paths

Let's say we have three directories: <span style="color: red;">Level-0</span>/<span style="color: yellow;">Level-1</span>/<span style="color: lime;">Level-2</span>.

From <span style="color: red;">Level-0</span>, `cd Level-1` will take you to <span style="color: yellow;">Level-1</span>.

From <span style="color: yellow;">Level-1</span>, `cd ..` will take you to <span style="color: red;">Level-0</span>.

From <span style="color: yellow;">Level-1</span>, `cd ./Level-2` will take you to <span style="color: lime;">Level-2</span>.

From <span style="color: lime;">Level-2</span>, `cd ../..` will take you to <span style="color: red;">Level-0</span>.

From <span style="color: red;">Level-0</span>, `cd Level-1/Level-2` will take you to <span style="color: lime;">Level-2</span>.

From <span style="color: yellow;">Level-1</span>, `cd .././Level-1/Level-2/..` will take you to <span style="color: yellow;">Level-1</span>.

----

This tutorial was last updated on Wednesday, May 14, 2025.
