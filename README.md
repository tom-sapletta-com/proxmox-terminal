# proxmox-terminal
Graphical terminal on Proxmox machine based on debian, X11, gnome, synergy, grid screen, auto tiling

## Menu

+ [Sources](#Sources)
+ [How To Install **Pop Shell** Window Tiling Extension](#How To Install **Pop Shell** Window Tiling Extension)
+ [Installing Material Shell]()
+ [Synergy]()
+ [Flatpak]()
+ [Add User]()
+ [Solaar]()

  
## Sources

+ [Leleat/Tiling-Assistant: An extension which adds a Windows-like snap assist to GNOME. It also expands GNOME's 2 column tiling layout.](https://github.com/Leleat/Tiling-Assistant)

+ [forge-ext/forge: Forge - Tiling and Window Manager for Gnome-Shell](https://github.com/forge-ext/forge)
Forge is a GNOME Shell extension that provides tiling/window management.

```bash
# X11
make test-x

# Wayland
make test-wayland

# Formatting, when you do npm install, 
# husky gets installed should force prettier formatting during commit
npm run format
```


## How To Install **Pop Shell** Window Tiling Extension 

+ [pop-os/shell: Pop!_OS Shell](https://github.com/pop-os/shell)
+ [Using Pop Shell on other GNOME Desktops - System76 Support](https://support.system76.com/articles/pop-shell/)
+ [How To Install Pop Shell Window Tiling Extension On Ubuntu 20.04, 20.10 Or 21.04, Fedora 32, 33 Or 34, Debian Bullseye Or Sid, And Arch Linux Or Manjaro - Linux Uprising Blog](https://www.linuxuprising.com/2020/05/how-to-install-pop-shell-tiling.html)



```bash
sudo apt install node-typescript make git
```


get the Pop Shell code from GitHub, build and install it for the current user on your GNOME 3.36, 3.38 or 40 desktop using:

```bash
git clone https://github.com/pop-os/shell
cd shell
make local-install
```


For Ubuntu / Debian, you can either download the Pop Shell Shortcuts DEB from here (it has no dependencies), or build it yourself as follows.

Install the Pop Shell Shortcuts dependencies:


```bash
sudo apt install cargo rustc libgtk-3-dev
```

clone the Pop Shell Shortcuts git repository, build and install it:

```bash
git clone https://github.com/pop-os/shell-shortcuts
cd shell-shortcuts
make
sudo make install
```


## Installing Material Shell


+ [Give Your GNOME Desktop a Tiling Makeover With Material Shell GNOME Extension](https://itsfoss.com/material-shell/)
+ [Material Shell - A new desktop experience](https://material-shell.com/#tiling-engine)


[Material Shell - A new desktop experience](https://material-shell.com/#persistence)

> # [](https://material-shell.com/#hotkeys)Hotkeys
> 
> Some hotkeys might already be used by GNOME Shell - please check your keybindings first.
> 
> #### [](https://material-shell.com/#desktop-navigation)Desktop navigation
> 
> - `Super+W` Navigate to the upper workspace.
> - `Super+S` Navigate to the lower workspace.
> - `Super+A` Focus the window at the left of the current window.
> - `Super+D` Focus the window at the right of the current window.
> - `Super+1`, `Super+2` ... `Super+0` Navigate to specific workspace
> 
> #### [](https://material-shell.com/#window-manipulation)Window manipulation
> 
> - `Super+Q` Kill the current window focused.
> - `Super+[MouseDrag]` Move window around.
> - `Super+Shift+A` Move the current window to the left.
> - `Super+Shift+D` Move the current window to the right.
> - `Super+Shift+W` Move the current window to the upper workspace.
> - `Super+Shift+S` Move the current window to the lower workspace.
> 
> #### [](https://material-shell.com/#extra-hotkeys)Extra Hotkeys
> 
> - `Super+Space` Cycle the tiling layout of the current workspace.
> - `Super+Escape` Toggle the UI of Material-shell, like a Zen mode.


## Synergy

+ [Download Synergy 3](https://symless.com/synergy/download)
+ 

## Flatpak


```bash
apt install flatpak
# Install the Software Flatpak plugin
apt install gnome-software-plugin-flatpak
# Add the Flathub repository
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
reboot
```
    


## Add User

the usermod command with the -a (append) and -G (group name) options to add users to sudoers. 
The -G option allows us to name the group we’d like to add the user to, and the -a option tells usermod to add the new group to the list of existing groups this user is already in.
make sure you’ve included the -a option.
```
sudo usermod -aG sudo tom
```

We need to edit the sudoers file.

```bash
sudo visudo
```

Add these lines below that section

```
# user tom can install software
tom     ALL=(root) /usr/bin/apt
```



## Solaar

+ [pwr-Solaar/Solaar: Linux device manager for Logitech devices](https://github.com/pwr-Solaar/Solaar)

+ [Manual Installation | Solaar](https://pwr-solaar.github.io/Solaar/installation)
  
```
# An easy way to install the most recent release version of Solaar is from the PyPI repository. First install pip, and then run
pip install --user 'solaar[report-descriptor,git-commit]'

# This will not install the Solaar udev rule, which you will need to install manually by copying
~/.local/share/solaar/udev-rules.d/42-logitech-unify-permissions.rules
# to /etc/udev/rules.d as root.
```
 
