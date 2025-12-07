# Dotfiles

Register alias:

`git config --global alias.df '!git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'`

Clone bare: 

`git clone --bare git@github.com:davidramiro/dotfiles.git $HOME/.dotfiles`

Ignore untracked:

`git df config --local status.showUntrackedFiles no`

Checkout:

`git df checkout`
