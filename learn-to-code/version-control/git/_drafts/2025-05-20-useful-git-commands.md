---
title: "useful git commands"
layout: post
---

<!-- TODO - add post front matter: useful git commands -->

<!-- TODO - add post content: useful git commands -->

# list git config settings

```shell
git config --list --show-origin
```

# set git config username

```shell
git config --global user.name "John Doe"
```

# set git config email

```shell
git config --global user.email email@example.com
```


# update the list of remote branches

This command will remove any remote branches that no longer exist in the remote repository.

```shell
git remote update --prune
```

```shell
git fetch --all
```

# update branches

```shell
git fetch
```

```shell
git fetch --all
```

```shell
git fetch --all --prune
```

# set merge behavior for pull

```shell
git config pull.rebase false
```

----

## resources and references

[Git Documentation - git fetch](https://git-scm.com/docs/git-fetch)
