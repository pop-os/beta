# Pop!_OS 20.04 Beta Testing

Thank you for participating in Pop!\_OS 20.04 beta release testing. This release brings major new features including Pop!_Shell tiling and the Flathub software repository. There are many corner cases with both of these technologies that your testing will help reveal.

This video provides an introduction to the tiling feature: https://youtu.be/-fltwBKsMY0

This workspaces video describes new keyboard shortcuts: https://youtu.be/v9oVZwJrjOc

**THIS IS A BETA**. Bugs are expected and re-installs likely.

If you experience trouble upgrading to the 20.04 beta with the `pop-upgrade` utility, it may be fixed by dropping to a TTY terminal ( <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>F3</kbd> ) and running the following commands:
```
sudo apt -f install
sudo apt full-upgrade
```
and then rebooting your machine. 

## Testing and Reporting Issues

We're seeking upgrade testing as well as fresh install testing. You can upgrade to 20.04 from Pop!\_OS 18.04 and 19.10. If you're on 19.04 you must first upgrade to 19.10. It is recommended that you backup your data, download the Pop!\_OS 20.04 Beta ISO and write it to a USB drive first.

Pop!_OS 20.04 Beta ISO is located here:

[Intel/AMD](https://pop-iso.sfo2.cdn.digitaloceanspaces.com/20.04/amd64/intel/4/pop-os_20.04_amd64_intel_4.iso)


[NVIDIA](https://pop-iso.sfo2.cdn.digitaloceanspaces.com/20.04/amd64/nvidia/4/pop-os_20.04_amd64_nvidia_4.iso)

Upgrade from 18.04 and 19.10 to 20.04 with the command:
```
sudo pop-upgrade release upgrade systemd -f
```

Upgrade from 19.04 to 20.04 by first upgrading to 19.10 with the command:
```
sudo pop-upgrade release upgrade systemd
```

After the successful upgrade to 19.10, you can then upgrade to 20.04 with the command:
```
sudo pop-upgrade release upgrade systemd -f
```

If you encounter issues running the `pop-upgrade` command, in a second terminal window, run the command:
```
sudo pop-upgrade daemon
```
And then run the upgrade command again.

## Reporting Issues

Report issues you encounter on this repository. Label issues with the `20.04` tag. Issues will be triaged and added to the Pop!\_OS 20.04 project.

## Pop!_OS 20.04 Beta Release Notes

To advance keyboard driven control, keyboard shortcuts have been modified in Pop!_OS 20.04.

### Notable Shortcut Changes

|          Action            |     Old Shortcut      |      New Shortcut  |
|:---------------------------| :-------------------- |--------------------|
Lock Screen                 | Super + L             | Super + Escape |
Move to Workspace Up or Down | Super + Up/Down Arrow | Super + Ctrl + Up/Down Arrow
Close Window                 | Super + W             | Super + Q
Toggle Maximize              | Super + Up Arrow      | Super + M

### New Features

#### Pop Shell Tiling
Pop!_OS 20.04 features automatic window tiling. To activate tiling mode, click the tiling menu icon at the top right of the screen and toggle on Tile Windows. Open and newly launched windows will be automatically tiled. Toggling off Tile Windows will revert to floating mode.

Click the tiling menu icon again and choose Keyboard Shortcuts. This help application will show you how to navigate, move, and resize windows all with your keyboard.

#### New Application Switcher and Launcher
Type `Super` + `/` to activate the new application switcher and launcher. Instead of `Super` + `Tabbing` through application icons, simply type `Super` + `/` and start typing the name of the application you want to switch to or launch.

#### Flatpak support with the Flathub
Pop!_Shop now includes Flatpak application support and the Flathub application repository by default. The source of applications is visible when viewing applications details.

System76 continues to curate and package key applications such as Steam, Atom, and VS Code. Pop!_OS repositories are prioritized to provide the best user experience for these applications.

Please use the Flathub version of applications not in the Pop!_OS repository. We're very interested in learning if you encounter issues.

If you use scripting for applications such as GIMP and KiCAD, the debian package is recommended.

