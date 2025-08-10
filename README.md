
# Personal Ansible Setup
A Ansible Script that download my Arch Desktop setup and homelab setup? (To Be Work on). basically just download alot of basic package for desktop usage as well the dotfiles I use (found in this [repo](https://github.com/TriforceGB/.dotfiles))


## Features

- Select from 3 presets (Base, Desktop, Server)
    - Base: Just changes to Terminal Usage such as install zsh and plugins
    - Desktop: install Base + packages and dots for Desktop or laptop Usage
    - Server: Install Base + packages needed for running an homeserver (not working rn)
     
- It will also install the related dots for the presets from my dotfiles repo

## Usage
To run the Ansible Setup just run this command to install the needed packages and then run the Ansible Script 
```
bash -c "$(curl -fsSL https://raw.githubusercontent.com/TriforceGB/Ansible-Playbook/main/Scripts/Pre-Ansible.sh)"
```

## Package List
### Base
#### zsh + stuff needed for plugins
- zsh
- zoxide
- eza
- tmux
#### Fonts
- otf-firamono-nerd
- noto-fonts
- noto-fonts-cjk
- noto-fonts-emoji
- fzf
#### Terminal Editors
- nano
- vim
- neovim
- vi (for visudo could remove later)
- github-cli
#### File Management and view
- less
- bat
- superfile
#### System View
- htop
- btop
#### python
- python
- uv
#### Terminal programs
- fastfetch
- tldr
- cmatrix
- tailscale
- bind-tools
### Desktop
#### Basic Workstations Needs
- kitty
- gnome-disk-utility
- timeshift
- zen-browser-bin
- vesktop-bin
#### Boot
- grub
- sddm
- qt6
- qt6-svg
- qt6-virtualkeyboard
- qt6-multimedia
- qt6-multimedia-ffmpeg
#### Nautilus & Extensions
- nautilus
- sushi
- nautilus-image-converter
- imagemagick
- folder-color-nautilus
- nautilus-open-any-terminal
- nautilus-admin-gtk4
#### Editor and Viewer
- audacity
- gimp
- gnome-text-editor
- mission-center (Task Manager)
- libreoffice-fresh
- loupe
- obs-studio
- vlc
- zed
- visual-studio-code-bin
#### Password Manager
- fuzzel
- rbw
- rofi-rbw
- bitwarden-bin
#### Gaming
- steam
- lutris
- prismlauncher
- wootomation-appimage
#### Others
- obsidian
- syncthing
- qbittorrent
- vulkan-tools
- qalculate-gtk
- archlinux-tweak-tool-git
- localsend
- parabolic
- upscayl-bin
- mesa
- vulkan
## Todo
- finalize the package install list
- make the dots being install a separate flag so you can just install the package but not the dotfiles
- create the file for server (might wait until I redo the homeserver)
- unhardcode some personal info such as email
