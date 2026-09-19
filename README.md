# dotfiles

This repository is managed as a **bare Git repository** so your home directory can be the working tree.

## Setup

```bash
git clone --bare git@github.com:Houndoom96/dotfiles.git $HOME/.dotfiles
alias dotfiles='git --git-dir=$HOME/.dotfiles --work-tree=$HOME'
dotfiles config --local status.showUntrackedFiles no
```

## Usage

Use `dotfiles` instead of `git` for tracking files in `$HOME`:

```bash
dotfiles status
dotfiles add .zshrc
dotfiles commit -m "Update zsh config"
dotfiles push
```
