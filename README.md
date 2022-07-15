# Dmenu Scripts (dmenuscripts, modified version of dmscripts by distrotube, but dm-logout is for openrc and some of the scripts adjusted to my needs)

The scripts included in this repo are:

- dm-confedit - Choose from a list of configuration files to edit.
- dm-logout - Logout, shutdown, reboot or lock screen.
- dm-maim - A GUI to maim using dmenu.
- dm-wifi - Connect to wifi using dmenu.
- \_dm-helper.sh Helper scripts adding functionality to other scripts

# Dependencies

Of course, dmenu is a dependency for all of these scripts. To see the dependencies of each individual script, check the top commented block of text in each script. For installing you will need pandoc and, of course, git.

# Installation

if u want to install this, you can simply clone and do `sudo make install` inside the cloned repo, or by adding my custom [arch repo](https://gitlab.com/samuelnihbos/samuel-arch-repo) and do `sudo pacman -Syyu && sudo pacman -S dmenuscripts`
