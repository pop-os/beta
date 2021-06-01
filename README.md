# Pop!\_OS 21.04 Beta Testing

Thank you for participating in Pop!\_OS 21.04 beta release testing! This release brings major new changes to the Desktop Environment including customization options with COSMIC. There are many corner cases with those features that your testing will help reveal.

**THIS IS A BETA**. Bugs are expected and re-installs likely.

## Installing or Upgrading

We're seeking upgrade testing as well as fresh install testing. You can upgrade to Pop!\_OS 21.04 from Pop!\_OS 20.10. It is recommended that you backup your data, download the Pop!\_OS 21.04 Beta ISO and write it to a USB drive first.

Pop!\_OS 21.04 Beta ISO is located here:

[Intel/AMD](https://pop-iso.sfo2.cdn.digitaloceanspaces.com/21.04/amd64/intel/2/pop-os_21.04_amd64_intel_2.iso)

[NVIDIA](https://pop-iso.sfo2.cdn.digitaloceanspaces.com/21.04/amd64/nvidia/2/pop-os_21.04_amd64_nvidia_2.iso)

Upgrade from Pop!\_OS 20.10 to Pop!\_OS 21.04 with the command:
```
sudo pop-upgrade release upgrade -f
```

If you encounter issues running the `pop-upgrade` command, you can view the daemon logs with the command:

```
sudo journalctl -u pop-upgrade
```

Alternatively, in a second terminal window you can stop the system daemon and then run the daemon in the foreground with the commands:

```
sudo systemctl stop pop-upgrade
sudo pop-upgrade daemon
```
and then run the upgrade command again. When you are finished, you can restart the system daemon with the command:

```
sudo systemctl start pop-upgrade
```

## Reporting Issues

Report issues you encounter on this repository. Label issues with the `21.04` tag. Issues will be triaged and added to the Pop!\_OS 21.04 project. If you have any usability feedback, label issues with ux tag or contact our UX architect at ux@system76.com.

## Release Notes

Release notes will be added soon
