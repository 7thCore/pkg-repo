# 7thCore's script repository

By installing the repository you will also be able to update the script using the package manager when a new update is available.

**Arch based distro**

Edit `/etc/pacman.conf`and add the following line to the bottom of the file:

```
Include = /etc/pacman.d/seventhcore-scripts-repo
```

Then create a new file at `/etc/pacman.d/seventhcore-scripts-repo` and add the following content:

```
[seventhcore-scripts-repo]
SigLevel = Optional TrustAll
Server = https://raw.githubusercontent.com/7thCore/pkg-repo/pkg-arch
```

Arch users have to install steamcmd from the aur before attempting to install the package.

You can now install the script by running `pacman -Sy arma3srv-script`

**Debian based distro**

Then create a new file at `/etc/apt/sources.list.d/seventhcore-scripts-repo.list` and add the following content:

```
deb https://raw.githubusercontent.com/7thCore/pkg-repo/pkg-debian stable main
```

You can now install the script by running `apt update` and after that `apt install arma3srv-script`

-------------------------
