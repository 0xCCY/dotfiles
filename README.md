# 0xCCY's dotfiles
Currently this is the dotfiles used by me to instantiate a new WSL2 distro (Ubuntu LTS).

# Installation
Run the following comman in the distro:
```
 curl -Lks https://raw.githubusercontent.com/0xCCY/dotfiles/master/.install | /bin/bash
```
*Note:*
1. Can be further shorten with link shortener
2. The `curl` params are optional. 
```
L - Follows redirect (this allow link shortener but since I cannot find a free one I use the "raw" url from GitHub
k - Bypass SSL (not sure why sometimes without this it will fail with SSL check)
s - Silent mode so nothing is being Echo when downloading (turn this off for debugging)
```

# What each files does?
## 1. install.sh
This is the entry point of the script. By requesting this script via curl, it will auto install the apt-packages, run commands and 

There are two ways to add new packages:
- Add the package name to the variable `apt_packages`
- Add in the installation commands in the `customize()` function. (Some packages like Oh My Zsh cannot be install via apt-get)

## 2. .zshrc
This is where ZSH config is stored, mostly Alias.

## 3. .p10k.zsh
This is the theme config of Power Level 10k Oh My ZSH theme.
 
# Changelog
## V0.1
Project initialized! Nothing fancy here just trying things out.
