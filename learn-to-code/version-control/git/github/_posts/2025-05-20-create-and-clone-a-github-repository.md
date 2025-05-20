---
layout: post
author: brittni watkins
date: 2025-05-20 20:00:00 -0000
modified_date: 2025-05-20
title: "create and clone a github repository"
excerpt: "In this tutorial, we will walk through how to create a new GitHub repository and how to clone the repository to our local machine."
tags:
  - git
  - github
  - clone
  - repository
  - new repository
---

[GitHub](https://github.com/) “is a developer platform that allows developers to create, store, manage and share their code...providing the distributed version control of Git”. Using Git and GitHub together, a developer can update their code, track changes, create issues, build deployment workflows, and review and accept changes to their code from developers around the world.

In this tutorial, we will walk through how to create a new GitHub repository and how to clone the repository to our local machine.

To complete this tutorial, you will need the following:

1. A [GitHub](https://github.com/) account
1. A Unix shell program installed on your computer. Additional information about Unix shell programs can be found in the [useful unix commands guide]({% post_url learn-to-code/unix/2025-05-14-useful-unix-commands %}).
1. Git installed on your computer. Additional information about installing Git can be found in the [git installation guide]({% post_url learn-to-code/version-control/git/2025-05-13-how-to-install-git %}).

----

## table of contents

[local repository vs. remote repository](#local-repository-vs-remote-repository)

----

## local repository vs. remote repository

Before we create a new repository, we need to understand the difference between a local repository and a remote repository, and how we use Git and GitHub together to maintain the two.

A local repository is code in a folder on your computer. This is the code that we will be editing, saving, running, testing, and debugging during the development process. You do not need a network connection to access this code, because all of the files are downloaded and saved on your computer.

A remote repository is code that resides on some remote server. In this case, the code will be held on GitHub servers. You can interact with this code via the GitHub website, and you can run, test, and debug the code using [GitHub Codespaces](https://docs.github.com/en/codespaces). Accessing a remote repository always requires a network connection because accessing the code requires access to the GitHub website.

It is possible to have a local repository that does not have a corresponding remote repository on GitHub, and it is possible to have a remote repository on GitHub that does not have a corresponding local repository on your computer.  For this tutorial, we will be creating a remote repository on the GitHub website, and cloning that remote repository so that we have a corresponding local repository on our computer.

After cloning the remote respository, changes to the local repository will not be synced automatically to the remote repository, nor vice versa. Once a repository has been cloned, we must use Git to indicate which files and changes should be synced between the local and remote repositories.

*A guide on useful git commands is coming soon!*

<!-- TODO - link to useful git commands post -->

----
