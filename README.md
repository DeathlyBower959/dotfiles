
# dotfiles

my arch linux config files :)

## Packages

cava - Cross-platform Audio Visualizer
fastfetch - System information tool
fish - Shell
htop - Process viewer
hyprdots - Starter hyprland desktop environment (DE) ~ Remove in the future
hypr - Window manager (WM)
kitty - Terminal
waybar - Wayland taskbar for sway
yay - AUR helper

## Setup
```sh
git clone --depth 1 https://github.com/prasanthrangan/hyprdots ~/HyDE
cd ~/HyDE/Scripts
./install.sh

alias dotfiles='usr/bin/git --git-dir=$HOME/.dotfiles --work-tree=$HOME'
git clone --bare https://github.com/deathlybower959/dotfiles.git $HOME/.dotfiles
dotfiles checkout
```


## System

Super + Q -> Close active window
Super + Delete -> Lock screen
Super + Shift + Delete -> Kill hyprland
Super + Backspace -> Logout/power screen
Super + O -> Toggle split
Super + F -> Browser (Firefox)
Super + Space -> Terminal
Super + / -> Keybind hint
Alt + Space -> Application launcher


## Terminal (kitty) ~/.config/kitty/

fish - Shell of the terminal ~/.config/fish/config.fish
fastfetch - System information manager ~/.config/fastfetch


## Packages

pacman -Sy -> Sync the package registry
pacman -Syu -> Upgrade all packages
pacman -S NAME -> Install/upgrade package

yay (pacman wrapper)

## Window Manager (hyprland / wayland) ~/.config/hypr/

Super + 1 -> Workspace 1
Super + Shift + 1 -> Move to workspace 1
Super + Shift + Ctrl + Arrow -> Move active window around current workspace
Super + J -> Toggle current split (horiz/vert)

Super + Arrow -> Move between windows


## Neovim

Stuff?

TODO
- Make cursor more visible
- Basic language setup
- Any git integrations?
- Simple file navigation


## Theming (hyde) ~/.config/hyde/

Cappuchin Mocha
https://github.com/prasanthrangan/hyprdots


## Split Monitor Workspaces (https://github.com/Duckonaut/split-monitor-workspaces)

Installed with hyprpm


## Dotfiles

Intitalized with:
git init --bare $HOME/.dotfiles
alias dotfiles='usr/bin/git --git-dir=$HOME/.dotfiles --work-tree=$HOME'
dotfiles config --local status.showUntrackedFiles no

dotfiles status
dotfiles add .vimrc
dotfiles commit -m "Add vimrc"
dotfiles push

### Setup

alias dotfiles='usr/bin/git --git-dir=$HOME/.dotfiles --work-tree=$HOME'
git clone --bare https://github.com/deathlybower959/dotfiles.git $HOME/.dotfiles
dotfiles checkout