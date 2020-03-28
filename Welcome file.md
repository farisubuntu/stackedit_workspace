# https://gparted.org/livecd.php:



# Live CD/USB/PXE/HD

**GParted Live** is a small bootable GNU/Linux distribution for x86 based computers.  
It enables you to use all the [features](https://gparted.org/features.php) of the latest versions of the GParted application.  
  
GParted Live can be installed on CD, USB, PXE server, and Hard Disk then run on an x86 machine.  

**CAUTION**: Creating a whole disk or partition image backup is recommended before you resize or move a partition. Some free software (GPL) disk and partition image tools are available:  
  
[Clonezilla](http://clonezilla.org), [doClone](http://doclone.nongnu.org), [FSArchiver](http://www.fsarchiver.org), [G4L](http://g4l.sourceforge.net), [g4u](http://www.feyrer.de/g4u), [Partimage](http://partimage.org), [Partclone](http://partclone.org).

## Installation Instructions

To install GParted Live on CD, [download](https://gparted.org/download.php) the .iso file and burn it as an image to a CD.  
  
For other installations, please refer to the following documents:  
[GParted Live on USB](https://gparted.org/liveusb.php)  
[GParted Live on PXE server](https://gparted.org/livepxe.php)  
[GParted Live on Hard Disk](https://gparted.org/livehd.php)  
[Add packages in GParted Live](https://gparted.org/add-packages-in-gparted-live.php)  
[Create your own custom GParted Live from scratch](https://gparted.org/create-gparted-live.php)  

## Usage Instructions

See the [GParted Live Manual](https://gparted.org/display-doc.php?name=gparted-live-manual) for instructions on how to use the Live image.  
See the [GParted Manual](https://gparted.org/display-doc.php?name=help-manual) for instructions on how to use the application for partitioning tasks.  
See the [documentation](https://gparted.org/documentation.php) page for copies of the GParted Manual in other languages.

## Accounts in GParted live

GParted live is based on [Debian live](http://live.debian.net/), and the default account is "user", with password "live". There is no root password, so if you need root privileges, login as "user", then run "sudo" to get root privileges.

## Available boot parameters

You can find the available boot parameters for GParted live [here](https://gparted.org/gparted-live-boot-param.php).

## Included Packages

GParted Live includes additional packages, such as:  

### Graphical Utilities

Right click on the desktop to access a pop-up menu.

Program

Description

[lxterminal](http://wiki.lxde.org/en/LXTerminal)

Terminal emulator (provides access to command line)

[pcmanfm](http://pcmanfm.sourceforge.net/)

Graphical file manager

[leafpad](http://tarot.freeshell.org/leafpad/)

Graphical text editor

[netsurf](http://www.netsurf-browser.org/)

Small web browser

[gsmartcontrol](http://gsmartcontrol.sourceforge.net/)

Hard disk drive and SSD health inspection tool

[calcoo](http://calcoo.sourceforge.net/)

RPN and algebraic scientific calculator

### Command Line Utilities

Program

Description

[fsarchiver](http://www.fsarchiver.org/)

File system archiver and restorer  

[partclone](http://partclone.org/)

Backup partitions into a compressed image file (e.g., partclone.ext4)

[partimage](http://www.partimage.org/)

Backup partitions into a compressed image file  

[testdisk](http://www.cgsecurity.org/wiki/TestDisk)

Data recovery tool that can help recover lost partitions  

[gpart](http://en.wikipedia.org/wiki/Gpart)

(Older) data recovery tool that can help recover lost msdos partition tables  

[grub](http://www.gnu.org/software/grub/)

GRand Unified Bootloader for restoring GRUB 2 boot loader  

[mc](http://www.gnu.org/software/mc/)

Text based file manager known as Midnight Commander

[nano](http://www.nano-editor.org/)

Text editor

[vim-tiny](http://www.vim.org/)

Enhanced vi text editor

[parted](http://www.gnu.org/software/parted/)

Partition table editor

[fdisk](http://en.wikipedia.org/wiki/Util-linux)

MSDOS partition table editor

[sfdisk](http://en.wikipedia.org/wiki/Util-linux)

MSDOS partition table editor also useful to save/restore partition table to/from a file

[gdisk](http://sourceforge.net/projects/gptfdisk/)

GPT partition table editor

[sgdisk](http://www.rodsbooks.com/gdisk/sgdisk.html)

GPT partition table editor also useful to save/restore partition table to/from a file

[gptsync](http://packages.debian.org/sid/gptsync)

GPT and MSDOS partition tables synchronization tool useful for Mac OS X users

[openssh](http://www.openssh.com/)

Secure shell (ssh) connectivity tool suite

[screen](http://www.rackaid.com/blog/linux-screen-tutorial-and-how-to/)

Screen manager with VT100/ANSI terminal emulation

[ping](http://linux.die.net/man/8/ping)

Check network connectivity to another host on a network

[rsync](http://linux.die.net/man/1/rsync)

Fast, versatile, remote (and local) file-copying tool

[telnet](http://linux.die.net/man/1/telnet)

Communicate with another host using the TELNET protocol

[traceroute](http://linux.die.net/man/8/traceroute)

Print the route packets trace to network host

[bc](http://linux.die.net/man/1/bc)

Arbitrary precision calculator language

To view all of the included packages you can either:  
refer to the "packages-_x.y.z_-_w_.txt" file in the download directory,  
or  
view the file "live/packages.txt" file inside the GParted Live iso file or zip file.

# To be embed into Linux_Cheateshet
\

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTI0NDY5MzY5N119
-->