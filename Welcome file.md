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
# GParted, Partition, and Filesystem Flags
[Jul 19, 2015](https://www.linux.org/threads/gparted-partition-and-filesystem-flags.11640/post-41005)

-   [#1](https://www.linux.org/threads/gparted-partition-and-filesystem-flags.11640/post-41005)

When using Parted, Gparted, fdisk, and other similar software, many people have noticed the "flags". What are these and what do they mean?  
  
Flags indicate that a certain property, characteristic, or feature is active or is present. Flags can either be on or off. If the flag is not seen, then it is off or inactive/non-existent. Certain flags are only supported on particular filesystems and partitioning tables. The GUID Partitioning Table (GPT) and MS-DOS partitioning table support the most flags. The flags (on GPT) are actually 128-bit GUIDs on the GUID partitioning table. Each flag has its own GUID.  
  

![gparted-flags.jpg](https://www.linux.org/attachments/gparted-flags-jpg.2533/)

  
  
Parted can be used to format a storage device with a particular partitioning table (also called a "disk-label"). Doing so will erase all partitions and data on the selected storage device. The command is "parted mklabel DISKLABEL". The command requires Root privileges. The user will need to create new partitions for the storage device. Supported partitioning tables (supported by parted) include the listed below.  

-   bsd
-   loop (raw disk access)
-   gpt
-   mac (Apple Partition Map (APM))
-   msdos (commonly called MBR)
-   pc98
-   sun

  
NOTE: Other partitioning tables exist, but parted does not support all of them.  
  
To configure a flag on a partition, the parted command is "parted set PARTITION# FLAG ON/OFF". Use this command with Root privileges. For example, to set partition 3 as the boot partition, the command would be "parted set 3 boot on". The flag name is case-sensitive.  
  
Below are descriptions and explanations for many flags as well as a list of the partitioning tables that support it (in brackets). This may not be a complete list of flags.  
  

-   atvrecv - [GPT] This is a flag for Apple TV Recovery Partitions.
-   bios_grub - [GPT] The partition with this flag is used as the GRUB BIOS partition. The partition usually uses about a megabytes of space and is not needed by EFI-booting systems.
-   boot - [Mac, MS-DOS, GPT, PC98] This flag indicates that the partition is bootable. On MS-DOS partitioning tables, only one partition may have this flag. However, other partitioning tables allow multiple partitions to have this flag.
-   DIAG - [MS-DOS] The partition is used for recovery and diagnostics.
-   esp - [MS-DOS, GPT] This flag indicates an UEFI System Partition. GPT uses this flag as an alias for "boot". The UEFI firmware stores files on this partition.
-   hidden - [MS-DOS, PC98] Partitions with this flag are hidden from Microsoft operating systems.
-   hp-service - [GPT] This the flag for HP Service Partitions. This partition uses the FAT filesystem.
-   irst - [MS-DOS, GPT] Intel Rapid Start Technology partitions use this flag.
-   lba - [MS-DOS] This flag is used by DOS, Windows 9x, and Windows ME and tells the system to use Linear Mode (Logical Block Addressing).
-   legacy_boot - [GPT] Some software (mostly legacy) recognize this flag as indicating that the GPT partition may be bootable.
-   LVM - [MS-DOS] This flag indicates to Linux that the partition is a physical volume.
-   msftdata - [GPT] This flag is applied to Microsoft Basic Data Partitions (BDP), such as NTFS and FAT filesystems including drive C:. This flag can only be removed if the flags "boot" or "msftres" is applied.
-   msftres - [GPT] Windows uses this flag to indicate a Microsoft Reserved Partition (MSR). This is only used on GPT partitioning tables and not MS-DOS (MBR) partitioning tables. Since GPT and the UEFI specification do not allow hidden partitions (exceptions apply), Microsoft Reserved Partitions are needed to replace hidden sectors sometimes used by Windows. Windows (on GPT) needs this partition and it must be before the primary and bootable partitions, but after the EFI System Partition (ESP) and OEM service partitions.
-   PALO - [MS-DOS] The marked partition can use the Palo bootloader (used by Linux/PA-RISC).
-   PREP - [MS-DOS, GPT] On PowerPC PReP and IBM RS6K/CHRP hardware, this flag indicates that the marked partition supports PReP booting. The PreP partition is not the same as the /boot/ directory or mountpoint.
-   raid - [MS-DOS] Linux recognizes this flag as a software RAID partition.
-   root - [MAC] This flag is used to inform Linux which partition is the root.
-   swap - [MAC] This is used to indicate that a swap partition is for a Linux system.
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTIyNjMxMjk3M119
-->