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

Git must have a configured username and email to associate with each commit made in your repositories. This configuration can either be set individually in each repository on your machine, or it can be set globally for every repository on your computer. The following instructions will walk through the global configuration.

If you are only using Git locally, the username and email that you set is inconsequential. However, if you are using a Git hosting service, such as [GitHub](https://github.com/) or [GitLab](https://about.gitlab.com/) your username and email should match those being used in the hosting service.

> [!CAUTION]
> The name and email you set in your configuration will be accessible to anyone who clones your repository or any repository you have contributed to.
> If you have a GitHub account, and would like to keep your email address private, you can configure your git email address to be the `noreply` email address provided by GitHub.
> Instructions on how to find your `noreply` email on GitHub are available in the [GitHub Docs: Setting your commit email address](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-email-preferences/setting-your-commit-email-address)

To set your Git configuration variables, open the Unix shell of your choice. On macOS, this will likely be the Terminal application. On Windows, this will likely be the GitBash application.

Type and execute the following commands:

```shell
git config --global user.name USER_NAME_HERE
```

```shell
git config --global user.email USER_EMAIL_HERE
```

You can double-check that the variables have been set with the following command:

```shell
git config --global --list
```

----

## resources and references

[Git](https://git-scm.com/)

[Git - Download for Linux and Unix](https://git-scm.com/downloads/linux)

[Git - Download for macOS](https://git-scm.com/downloads/mac)

[Git - Download for Windows](https://git-scm.com/downloads/win)

[Pro Git Book: First-Time Git Setup](https://git-scm.com/book/ms/v2/Getting-Started-First-Time-Git-Setup)

[GitHub Docs: Setting your commit email address](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-email-preferences/setting-your-commit-email-address)

----

This tutorial was last updated on Tuesday, May 20, 2025.
