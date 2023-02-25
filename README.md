# dotfiles
A list of dotfiles and configs I use with a simple setup for my terminal.

I use an Ubuntu base system.

My plugins for vim are `vim-airline` and `vim-monokai` and for `zsh`, `git`, `zsh-autosuggestions`, `z` and `sudo`.
Follow [`zsh-autosuggestions`](https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md#oh-my-zsh) to install it.

I also alias `nvim` with `vim` among some `tmux` shortcuts.

## tmux
Install [`tmux`](https://github.com/tmux/tmux).
```
apt install tmux
```
Copy `.tmux.config` file and restart terminal.

## zsh
Install `zsh` along side [`oh-my-zsh`](https://github.com/ohmyzsh/ohmyzsh)
```
sudo apt install zsh
```
Make it your default shell
```
sudo chsh -s $(which zsh)
```
Log out and log back in and install `oh-my-zsh`
```
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
Copy `.zshrc` file and restart terminal

## Neovim
Install [Neovim](https://github.com/neovim/neovim)
```
sudo apt install neovim
```
Install the [vim-plug](https://github.com/junegunn/vim-plug) Plugin Manager
```
sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
   https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
```
Copy `init.vim` file into new directory `~/.config/nvim`

Install the plugins
```
vim +PlugInstall
```
or enter `vim` and execute
```
:PlugInstall
```
Restart `vim`
### Done. ᕙ( ͡° ͜ʖ ͡°)ᕗ
