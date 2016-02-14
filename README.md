# Autoinstall

This package will produce a Debian installer ISO that is fully unattended.

Edit `preseed.txt` to taste, then run `make`. Copy `autoinstall.iso` to your VM provisioning system or burn it to a CD/DVD then boot.

On Linux the following are required:

* curl
* GNU make
* fuse
* genisofs
* rsync

On Debian/Ubuntu you can easyly install them with the command:

	sudo apt-get install curl make fuse genisoimage rsync fuseiso

On any OpenSolaris descendent (SmartOS, OmniOS, Oracle Solaris) the following ar
e required:

* curl
* GNU make
* mkisofs
* rsync

Override parameters using standard `make` variables.

### Examples

Build for i386.

    make ARCH=i386

Build a specific version

    make DEBIAN_VERSION=7.1.0

### Reference

Github:
* https://github.com/bahamat/debseed
* https://github.com/netson/ubuntu-unattended
* https://github.com/guessi/unattended_iso
* https://github.com/Tolsma/ubuntu-unattended
* https://github.com/netson/ubuntu-unattended

Preseed:
* https://www.debian.org/releases/stable/example-preseed.txt
* https://help.ubuntu.com/12.04/installation-guide/example-preseed.txt
* https://help.ubuntu.com/14.04/installation-guide/example-preseed.txt 

Divers:
* https://wiki.debian.org/DebianInstaller/Preseed/EditIso
* http://www.n0r1sk.com/index.php/Debian_Remaster_Netinstaller_-_Integrate_Firmware_bnx2x_and_Preseed

