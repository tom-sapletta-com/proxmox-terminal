# proxmox-terminal
Graphical terminal on Proxmox machine based on debian, X11, gnome, synergy, grid screen, auto tiling



## How To Install Pop Shell Window Tiling Extension 

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
