Use this wrapper script to install Arch on a SD card to be used in a Raspberry
Pi.

### Requirements
You must have `bsdtar`, `wget`, and `fdisk` installed for this script to run.
This script must be run as `root`.

### Usage
#### Determine the target device
Insert the SD card and use a command like `lsblk` to determine the name of the
SD card.  This is the `TARGET_DEV`.

#### Run the script
If you have a copy of the Arch-RaspberryPi tarball already, invoke the script as
follows:
```
# ./createSDCard TARGET_DEV PATH_TO.TAR.GZ
```
where replacing `PATH_TO.TAR.GZ` with the actual path to the tarball.

Otherwise, invoke the script as follows if you are preparing a SD card for a
Raspberry Pi 1:
```
# ./createSDCard TARGET_DEV 1
```
And if you have a Raspberry Pi 2:
```
# ./createSDCard TARGET_DEV 2
```

This script was tested on an Arch and Debian install.
