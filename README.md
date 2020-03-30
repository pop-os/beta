Thank you for participating in Pop!_OS 20.04 beta release testing. This release brings a major new features including Pop!_Shell tiling and the Flathub software repository. There are many corner cases to both of these technologies that your testing will help reveal.

We are conducting user testing with this beta release. If you are interested in participating in remote user testing with out UX architect *DO NOT INSTALL THE BETA YET*. Contact Maria @ maria@system76.com with your interest. We will be choosing up to 10 participants.

THIS IS A BETA. Bugs are expected and re-installs likely.

We seeking upgrade testing as well as fresh install testing. You can upgrade to 20.04 from Pop!_OS 18.04 and 19.10. If you're on 19.04 you must first upgrade to 19.10.

If you're upgrading, it is recommended that you backup your data, download the Pop!_OS 20.04 Beta ISO and write it to a USB drive first.

Pop!_OS 20.04 Beta ISO is located here:

Upgrade from 18.04 and 19.10 to 20.04
`sudo pop-upgrade release upgrade -f systemd`

Upgrade from 19.04 to 20.04
`sudo pop-upgrade release upgrade systemd`. After the successful updgrade, run `sudo pop-upgrade release upgrade -f systemd` to upgrade to the 20.04 beta.

Pop!_OS 20.04 Beta Release Notes

To advance keyboard driven control, keyboard shortcuts have been modified in Pop!_OS 20.04.

Notable Shortcut Changes

          Action             |     Old Shortcut      |      New Shortcut
Lock Screen                  | Super + L             | Super + Escape
Move to Workspace Up or Down | Super + Up/Down Arrow | Super + Ctrl + Up/Down Arrow
Close Window                 | Super + W             | Super + Q
Toggle Maximize              | Super + Up Arrow      | Super + M

New Features

Pop Shell Tiling
Pop!_OS 20.04 features automatic window tiling. To activate tiling mode, click the tiling menu icon at the top right of the screen and toggle on Tile Windows. Open and newly launched windows will be automatically tiled. Toggling off Tile Windows will revert to floating mode.

Click the tiling menu icon again and choose Keyboard Shortcuts. This help application will show you how to navigate, move, and resize windows all with your keyboard.

New Application Switcher and Launcher
Type Super + / to activate the new application switcher and launcher. Instead of Super+Tabbing through application icons, simply type Super + / and start typing the name of the application you want to switch to or launch.

Flatpak support with the Flathub
Pop!_Shop now includes Flatpak application support and the Flathub application repository by default. The source of applications is visible when viewing applications details.

System76 continues to curate and package key applications such as Steam, Atom, and VS Code. Pop!_OS repositories are prioritized to provide the best user experience for these applications.

If you use scripting for applications such as GIMP and KiCAD, the debian package is recommended.


