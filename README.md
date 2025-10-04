# system-setup

## some useful commands
- dnf info -> this will show the information for the package
- dnf info git -> will show the git package information
- fonts go in the .local/share/fonts/ -> put all the .ttf files here and then run fc-cache -f -v
- to list all the fonts installed use fc-list
- to filter out specific fonts use grep command -> fc-list | grep fontName
- there will be a .fonts.conf file in the ~ directory -> full path ~/.fonts.conf with something like below

```
<?xml version="1.0"?><!DOCTYPE fontconfig SYSTEM "fonts.dtd">
<fontconfig>
 <dir>~/.local/share/fonts</dir>
</fontconfig>
```

## configuration
- most of the configuration stays in the .config folder
- example ~/.config/nvim -> for neovim, ~/.config/Code -> for vscode
- To help manage the config files use symlinks and keep the files in a separate directory and mirror them in the .config folder. 
- [How to create a symlink](https://gist.github.com/JaySanSen/07f5855a7a0fe728f21d04240d972f85)

## which command
- this is used to locate the executable file associated with a command
- ex: which bash

```
~/Desktop/personal/system-setup$ which bash
/usr/bin/bash
```