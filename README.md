# .dotfiles

This repository contains my personal dotfiles.

Here is how I use this repository:
~~~
git init --bare /Volumes/Workspace/.dotfiles
alias config='/usr/bin/git --git-dir=/Volumes/Workspace/.dotfiles/ --work-tree=$HOME' # Already defined in .zshrc
config config status.showUntrackedFiles no

config status
config add .vimrc
config commit -m "Add vimrc"
config push
~~~
Reference: https://news.ycombinator.com/item?id=11071754
