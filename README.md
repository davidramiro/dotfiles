# Dotfiles

## Prerequisites:

- eza
- zoxide
- fzf
- nvim
- atuin
- zellij

## Setup

1. Register alias:

`git config --global alias.df '!git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'`

2. Add the following to `~/.gitconfig`:

```
[include]
    path = ~/.gitconfig-include
```

3. Clone bare: 

`git clone --bare git@github.com:davidramiro/dotfiles.git $HOME/.dotfiles`

4. Ignore untracked:

`git df config --local status.showUntrackedFiles no`

5. Checkout:

`git df checkout`

## Sync

`git df add file_to_sync && git df commit -m "something" && git df push`

