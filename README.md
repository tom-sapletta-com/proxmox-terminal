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

