# Pop!\_OS 22.04 LTS Beta Testing

Thank you for participating in Pop!\_OS 22.04 beta release testing!

**THIS IS A BETA**. Bugs are expected and re-installs are likely.

## Installing or Upgrading

We're seeking upgrade testing as well as fresh install testing. You can upgrade to Pop!\_OS 22.04 from Pop!\_OS 21.10. It is recommended that you backup your data, download the Pop!\_OS 22.04 Beta ISO and write it to a USB drive first.

Upgrading from 20.04 is possible, but `pop-upgrade` will first upgrade to 21.10, then you will need to upgrade again to get to 22.04. Support for upgrading directly to the 22.04 beta from 20.04 is actively being worked on.

Pop!\_OS 22.04 Beta ISOs are located here:

Intel/AMD Graphics ISO:
- [ISO](https://pop-iso.sfo2.cdn.digitaloceanspaces.com/22.04/amd64/intel/2/pop-os_22.04_amd64_intel_2.iso)
- [SHA256SUMS](https://pop-iso.sfo2.cdn.digitaloceanspaces.com/22.04/amd64/intel/2/SHA256SUMS)
- [SHA256SUMS.gpg](https://pop-iso.sfo2.cdn.digitaloceanspaces.com/22.04/amd64/intel/2/SHA256SUMS.gpg)

NVIDIA Graphics ISO:
- [ISO](https://pop-iso.sfo2.cdn.digitaloceanspaces.com/22.04/amd64/nvidia/2/pop-os_22.04_amd64_nvidia_2.iso)
- [SHA256SUMS](https://pop-iso.sfo2.cdn.digitaloceanspaces.com/22.04/amd64/nvidia/2/SHA256SUMS)
- [SHA256SUMS.gpg](https://pop-iso.sfo2.cdn.digitaloceanspaces.com/22.04/amd64/nvidia/2/SHA256SUMS.gpg)

Before upgrading an existing Pop!\_OS installation, run these commands to collect information about your system's installed sources and packages:
```
cat /etc/apt/sources.list >> sources.txt
ls -alh /etc/apt/sources.list.d/ >> sources.txt
cat /etc/apt/sources.list.d/* >> sources.txt
apt list --installed > packages.txt
```
Save these files in case they're needed to recreate any issues encountered while upgrading.

Then, upgrade from Pop!\_OS 21.10 to Pop!\_OS 22.04 with the command:
```
pop-upgrade release upgrade -f
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

Report issues you encounter on this repository. Issues will be triaged and added to the [Pop!\_OS 22.04 project](https://github.com/orgs/pop-os/projects/21). If you have any usability feedback, label issues with `ux` tag or contact our UX architect at ux@system76.com.

## Release Notes

Release notes will be available later.
