## Willow One Gtk Theme

Willow One is a flat Design theme for GTK 3, GTK 2 and Gnome-Shell which supports GTK 3 and GTK 2 based desktop environments like Gnome, Unity, Budgie, Cinnamon Pantheon, XFCE, Mate, etc.


## Info

### GTK+ 3.20 or later
- Set windows button on gnome for a better experience.

Gnome ≥ 3.22:

    gsettings set org.gnome.desktop.wm.preferences button-layout appmenu:minimize,maximize,close


### GTK2 engines requirment
- GTK2 engine Murrine 0.98.1.1 or later.
- GTK2 pixbuf engine or the gtk(2)-engines package.

Fedora/RedHat distros:

    dnf install gtk-murrine-engine gtk2-engines

Ubuntu/Mint/Debian distros:

    sudo apt-get install gtk2-engines-murrine gtk2-engines-pixbuf

ArchLinux:

    pacman -S gtk-engine-murrine gtk-engines

Other:
Search for the engines in your distributions repository or install the engines from source.

## Install

Usage:  ./install.sh  [OPTIONS...]

```sh
  -d, --dest DIR          Specify destination directory (Default: /home/vince/.themes)

  -n, --name NAME         Specify theme name (Default: Qogir)

  -t, --theme VARIANT     Specify theme primary color variant(s) [default|manjaro|ubuntu|all] (Default: blue color)

  -c, --color VARIANT     Specify theme color variant(s) [standard|light|dark] (Default: All variants)

  -i, --icon VARIANT      Specify logo icon on nautilus [default|manjaro|ubuntu|fedora|debian|arch|gnome|budgie|popos|gentoo|void|zorin|mxlinux|opensuse] (Default: mountain icon)

  -g, --gdm               Install GDM theme, this option need root user authority! please run this with sudo

  -l, --libadwaita        Install link to gtk4 config for theming libadwaita

  -r, --remove,
  -u, --uninstall         Uninstall/Remove installed themes

  --tweaks                Specify versions for tweaks [image|square|round] (options can mix use)
                          1. image:      Install with a background image on (Nautilus/Nemo)
                          2. square:     Install square window button like Windows 10
                          3. round:      Install rounded window and popup/menu version

  -h, --help              Show help


```

**FOR EXAMPLE:**

Install default themes

```sh
./install.sh
```

Install dark version

```sh
./install.sh -c dark
```

Install rounded window version with square window button and nautilus background image

```sh
./install.sh --tweaks image square round
```

Install standard dark gdm theme

```sh
sudo ./install.sh -g -c dark -t default
```

Uninstall gdm theme

```sh
sudo ./install.sh -g -r
```
# Willow-One-Dark
