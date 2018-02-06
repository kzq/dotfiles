# **Dotfiles**

A general store to sync development tools across multiple machines.

**Setting up new machine**
-------------------------

**Setup Dotfiles** <br />
On new machine, configure git repository to download dotfiles  
```ssh
cd ~ 

mkdir .dotfiles

git remote add origin https://github.com/kzq/dotfiles.git
```
**Atom**<br />
On new machine first install Atom and follow the steps below
```ssh
# move default .atom directory
mv ~/.atom/ ~/.dotfiles/ 

# create symbolic link
ln -s ~/.dotfiles/.atom/ ~/.atom

# sync settings
git pull origin master 

# open Atom, open Atom Command Palette (ctrl+shift+p) and install all packages
Package sync: Sync
```
