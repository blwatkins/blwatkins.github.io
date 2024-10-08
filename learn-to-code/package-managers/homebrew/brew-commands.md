# useful `brew` commands

----

# table of contents

[print the current version of `brew`](#print-the-current-version-of-brew)

[update `brew` to the latest version](#update-brew-to-the-latest-version)

[install a new package](#install-a-new-package)

[list all the installed packages](#list-all-the-installed-packages)

[uninstall a package](#uninstall-a-package)

[cleanup a package](#cleanup-a-package)

[cleanup all packages](#cleanup-all-packages)

[list all outdated packages](#list-all-outdated-packages)

[upgrade a package](#upgrade-a-package)

[upgrade all packages](#upgrade-all-packages)

[Fin.](#fin)

----

### print the current version of `brew`

```shell
brew --version
```

[table of contents](#table-of-contents)

----

### update `brew` to the latest version

```shell
brew update
```

[table of contents](#table-of-contents)

----

### install a new package

it is recommended to
[update `brew` to the latest version](#update-brew-to-the-latest-version)
before installing a new package.

replace `PACKAGE_NAME_HERE` with the name of the package to be installed.

```shell
brew install PACKAGE_NAME_HERE
```

[table of contents](#table-of-contents)

----

### list all the installed packages

```shell
brew list
```

[table of contents](#table-of-contents)

----

### uninstall a package

replace `PACKAGE_NAME_HERE` with the name of the package to be uninstalled.

```shell
brew uninstall PACKAGE_NAME_HERE
```

[table of contents](#table-of-contents)

----

### cleanup a package

replace `PACKAGE_NAME_HERE` with the name of the package to be cleaned up.

```shell
brew cleanup PACKAGE_NAME_HERE
```

[table of contents](#table-of-contents)

----

### cleanup all packages

```shell
brew cleanup
```

[table of contents](#table-of-contents)

----

### list all outdated packages

```shell
brew outdated
```

[table of contents](#table-of-contents)

----

### upgrade a package

if there is a new version of `brew` available,
you may need to
[update `brew` to the latest version](#update-brew-to-the-latest-version)
before you can upgrade the package.

replace `PACKAGE_NAME_HERE` with the name of the package to be upgraded.

```shell
brew upgrade PACKAGE_NAME_HERE
```

[table of contents](#table-of-contents)

----

### upgrade all packages

if there is a new version of `brew` available,
you may need to
[update `brew` to the latest version](#update-brew-to-the-latest-version)
before you can upgrade the packages.

```shell
brew upgrade
```

[table of contents](#table-of-contents)

----

### Fin.

[table of contents](#table-of-contents)
