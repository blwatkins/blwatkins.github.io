---
layout: post
author: brittni watkins
date: 2025-06-10 12:00:00 -0000 # Update this date to the current date
modified_date: 2025-06-10
title: "editing files in vi"
excerpt: "In this guide, we will cover the basics of using vi to edit files in  a Unix shell."
tags:
  - unix
  - command line
  - shell
  - bash
  - z shell
  - vi
---

`vi` is a screen-oriented text editor originally created for the Unix operating system. In this guide, we will cover the basics of using `vi` to edit files in a Unix shell. This is not an exhaustive guide.

All `vi` commands will be executed using a command line interface (CLI) application running a Unix shell instance, such as `bash` or `zsh`.
Additional information about command line interface applications can be found in the
[software for unix guide]({% post_url learn-to-code/unix/2025-05-21-software-for-unix %}).
Additional information about executing Unix shell commands can be found in the
[useful unix commands guide]({% post_url learn-to-code/unix/2025-05-14-useful-unix-commands %}).

----

## table of contents

[opening a file in vi](#opening-a-file-in-vi)

[insert mode](#insert-mode)

[command mode](#command-mode)
- [commands](#commands)
  - [`:w`](#save-your-file-write)
  - [`:q`](#exit-vi-quit)
  - [`:wq`](#save-and-exit-write-and-quit)

[resources and references](#resources-and-references)

----

## opening a file in vi

```shell
vi FILEPATH_HERE
```

The `vi` command opens the specified file in the `vi` text editor. If the file does not exist, it will be created when you save your changes.

The provided file path can be an absolute path or a relative path.
Additional information about file paths can be found in the
[absolute and relative paths guide]({% post_url learn-to-code/unix/2025-05-14-absolute-and-relative-paths %}).

----

## insert mode

When you open a file in `vi`, the file opens in command mode by default. To edit the file, you will need to switch to insert mode.

To switch to insert mode from command mode, press the `i` key on your keyboard. You can now type and edit the file as needed.

To return to command mode from insert mode, press the `ESCAPE` key on your keyboard. You will need to return to command mode to save your changes or exit `vi`.

----

## command mode

In command mode, you cannot type or edit the file directly.
Instead, you will use various commands and keystrokes to manipulate the file.
In command mode, you can perform actions such as saving the file, exiting `vi`, deleting lines, copying lines, and more.

### commands

#### save your file (write)

```
:w
```

The `:w` command saves the changes you have made to the file without exiting `vi`.

To execute this command, type `:w` while in command mode, then press `ENTER`.

#### exit vi (quit)

```
:q
```

The `:q` command exits `vi` without saving any changes you have made to the file.

To execute this command, type `:q` while in command mode, then press `ENTER`.

#### save and exit (write and quit)

```
:wq
```

The `:wq` command saves the changes you have made to the file and then exits `vi`.

To execute this command, type `:wq` while in command mode, then press `ENTER`.

----

## resources and references

[Wikipedia - vi (text editor)](https://en.wikipedia.org/wiki/Vi_(text_editor))

[Red Hat - An introduction to the vi editor](https://www.redhat.com/en/blog/introduction-vi-editor)
