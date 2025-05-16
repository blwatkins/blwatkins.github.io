---
layout: post
author: brittni watkins
date: 2025-05-13 22:00:00 -0000
title: "how to install git"
excerpt: "We have a few options for installing Git, and those options change depending on the operating system you are using.  In this tutorial, I will walk you through the installation process for Windows and macOS."
tags:
  - git
  - version control
  - installation
---

[Git](https://git-scm.com/) is a version control software that allows us to save and restore different versions of our files at various points. It is a powerful tool that allows us to track changes, collaborate with others, and manage our codebase effectively.

We have a few options for installing Git, and those options change depending on the operating system you are using.  In this tutorial, I will walk you through the installation process for Windows and macOS.  If you are using Linux, you can find download instructions for your specific distribution on the [Git website](https://git-scm.com/downloads/linux).

[git installation for windows](#git-installation-for-windows)

[git installation for macOS](#git-installation-for-macos)

[first time git setup](#first-time-git-setup)

----

## git installation for windows

You can find the official Git installation instructions for Windows on the [Git website](https://git-scm.com/downloads/win).

### > step 1

Download Git from the [Git website](https://git-scm.com/downloads/win).

### > step 2

Follow all instructions and prompts in the installation program.  Be sure to opt-in to installing the GitBash application. 

Windows does not come with a Unix shell command line interface (CLI) by default.  Installing GitBash will allow us to navigate through our operating system using common Unix shell commands that we would use with macOS or Linux machines.

### > step 3

Let's make sure the installation was successful.

Find and open the GitBash application. I recommend adding a shortcut to your Desktop or Start Menu, if one does not exist already.

Type and execute the following (hit `ENTER` or `RETURN` to execute the command):

```shell
git --version
```

Do you see a version number? If yes, congratulations! You have successfully installed Git!

----

## git installation for macOS

You can find the official Git installation instructions for macOS on the [Git website](https://git-scm.com/downloads/mac).  This tutorial will walk through the steps to install Git using [Homebrew](https://brew.sh/).

### > step 1

[Homebrew](https://brew.sh/) is a popular package manager used for managing software and package dependencies on macOS.

Find and open the Terminal application on your computer, then follow the steps on the [Homebrew website](https://brew.sh/) to install Homebrew.

### > step 2

Let's make sure the Homebrew installation was successful.

Find and open the Terminal application. I recommend adding a shortcut to your Desktop or Dock, if one does not exist already.

Type and execute the following (hit `ENTER` or `RETURN` to execute the command):

```shell
brew --version
```

Do you see a version number? If yes, congratulations! You have successfully installed Homebrew!

### > step 3

In the Terminal application, type and execute the following:

```shell
brew install git
```

### > step 4

Let's make sure the Git installation was successful.

In the Terminal application, type and execute the following:

```shell
git --version
```

Do you see a version number? If yes, congratulations! You have successfully installed Git!

----

## first time git setup

<!-- TODO - add first time git setup instructions -->
<!-- git config user.name -->
<!-- git config user.email -->
<!-- should match name and email in your Git host account -->
<!-- common git hosts -->
<!-- can set globally or for individual repositories -->

----

### resources and references

[Git](https://git-scm.com/)

[Git - Download for Linux and Unix](https://git-scm.com/downloads/linux)

[Git - Download for macOS](https://git-scm.com/downloads/mac)

[Git - Download for Windows](https://git-scm.com/downloads/win)

----

This tutorial was last updated on Wednesday, May 14, 2025.
