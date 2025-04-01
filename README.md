# First Linux-Installation

Comprehensive simple instructions for your first Linux-installation.

## Motivation

1. More & more people switch or want switch to Linux, the reasons why people wish this, will not be explained 
here, & i'm sure, if you search & found this page… you have already "found" your own motivation 😉.

2. My own motivation for doing these instructions… someone ask me & i cannot refuse/reject this request for a simple & 
important reason… 'the only & true meaning/sense of live': "Collecting knowledge & termless transfer to everybody".

### Step 1: Collect information & prepare your actual OS

* **Definitions**: we still have three kinds of Motherboards (MB), the very old BIOS, CMS & UEFI. CMS is a middle way 
between BIOS & UEFI & mean BIOS & UEFI Compatibility Support Module.

* Following points are (mostly) particularly dedicated to people "still using" **WinDoof** (shortcut WD), but, also 
important for Linux-Newbie.

* People that have already installed once Linux, this people can jump directly to **"§ 4. ot 5."**.

1. **Disable "Fast Start"** in WD System-settings, read/see correlated [How-to](Fast-Start_Function-on-WinDoof.md).

2. **Enable CMS** if present, read/see correlated [How-to](Find-CMS-in-BIOS.md).

3. **Disable "Secure-Boot"**, for this see/read correlated [How-to](Secure-Boot-in-BIOS-or-UEFI.md), read 
carefully dedicate note-s in last chapter of linked file/instructions.

4. **Considerations and/or recommendations**:
	* Linux can be installed also on computers having "Secure-Boot" enabled, but, i never done it & don't think it's a 
natural "situation" for a Linux-OS, besides… Linux don't ("yet") need it.
	* If a Linux installation should interfere with your "beloved" WinDoof installation or make it unusable... i 
recommend buying at least a refurbished mini computer like "Dell-Optiplex-7050-micro" or 7060 or equivalent.
	* If possible, please, use/get an additional Data-Carrier (DC) like a SATA-SSD or (better a) NVMe-PCIe or what-else 
DC-connection is available on your hardware (HW). Whitelist for recommended DC-s can be found 
[here](https://github.com/Advantaged/4Kn-Formatting/Whitelist-NVMe-PCIe.md)

### Step 2: Shrink (in case) your DC (Data-Carrier)

1. Best shrinking of WD-partitions through WD-own 'on-board-tools', read/see correlated 
[How-to](Shrink-WD-partition.md).

2. Alternatively you can user [GParted-Live](https://gparted.org/livecd.php) USB or similar tools based on Linux.

3. **Notes:**
	* Please let enough place on WD-main-partition for further use of the same.
	* WD must be restarted, no matter which tool you have used, that permits the changes to take effect and/or WD to 
recognize the new size. If you don't restart WD after shrinking, most probably you are not able anymore to use it.
	* Don't shrink any other WD-partition than the main partition "C:\" (or what-ever is called) & ***don't touch at 
all any WD-RAID***, those RAID-s are normally advertised with `RAID 0, 1, 5, 10`, the Linux-world call them 'fake-RAID' 
or 'software-RAID`. Once you touched such RAID in anyway, the RAID is done/gone❗️
	* If i remember me well, WD talk always about 'MB' (1000 KB) & not about 'MiB' (1024 KiB), outer after a WD-RAID 
creation, e.g. an HHD of 250 GB was represented as 250 GB when used as single DC but as 232 GB if used in a RAID.

### Step 3.: Choose the right Linux-Distro for you

There are a lot of Linux-Distribution in the digital world, see [Distro-Watch](https://distrowatch.com/) web-page, 
right-side, scroll ca. in the middle,you find it under menu "Page Hit Ranking" from 0 to 100, but there is much more.

* **My recommendations:**

1. If your hardware (HW) is not brand new but have already some years (3-4 or more) of work behind him, choose a 
**Regular (Point) Release Distros** like Kubuntu, Neon, Mint, Debian or any other popular Debian-Derivate.

2. If your HW is newer, i would choose a **Rolling Release Distros** & precisely (for me) the best OS worldwide 
names [CachyOS](https://wiki.cachyos.org/cachyos_basic/download/). Other distros like EndeavourOS, Garuda, Manjaro, 
etc. are also popular but… if you have high requirement to one OS or you are a gamer, you have at moment almost no 
other choice.

3. Choice of DE (Desktop-Environment). The DE is the appearances of an OS or precisely how/where the menus are 
displayed, where you find minimize, maximize, close & other buttons, how precisely you can change/modify the 
appearances, how detailed & deeply you can make your own settings, etc., etc..

3.1. **Plasma**-DE also called KDE, use "Qt", vector-graphic. The placement of menus & buttons is like under WD but 
very detailed, use many resources, can be modified in a very simple manner, the best `systemsettings` & appearances, 
not recommended for low-resources HW.

3.2. **Gnome**, use "Gtk", no vectorized pictures & graphics mainly. The placement of menus & buttons is like 
under an Apple desktop-OS, no so much adjustments/transformations-possibilities as Plasma but meanwhile also 
resources-hungry like Plasma, not recommended for low-resources HW.

3.3. **Lightweight**-DEs: If you HW is not so powerful, i recommend to use **LXQt** (Qt) or **XFCE** (Gtk) as DE. 
Many Distros offer plenty of DEs. If you are new to Linux, don't choose/use a 'Compositor'-DE that need a lot of manual 
adjustments in the CLI & configurations-files. The compositors practically offer you to build your own DE at your 
pleasure/wish. An incomplete list of DE can be found in linked [Linux-DE.md](Linux-DE.md)

### Step 4.: "Burn" a Linux-ISO on USB-stick

* For this purpose offer the [CachyOS-Wiki](https://wiki.cachyos.org/installation/installation_prepare/) very detailed 
& easy to follow/use explanations & examples for Apple, Linux & MicroSchrott (MS). As i in the Discord-channel of 
CachyOS understood, Balena-Etcher is at moment not working properly. The "Ventoy" tool, for Linux & WD permit you to 
store additional ISOs or other files like `*.md` (MarkDown) `*.txt` documents with instructions, etc.. **Note**: 
`*.md`-files like this can be opened also with normal text-editor or PDF-reader and so on.

* Furthermore, as i understood, also WD offer programs (six/6) like the "Linux-CLI" (Command-Line-Interface) that 
permit to use the `dd`-command like perfectly explained in the above-mentioned "CachyOS-Wiki". If you want make first 
experiences with the "CLI"… read/see correlated [How-to](CLI-under-WD.md) 😉.

* Use quality USB-sticks like SanDisk, my first bought sticks, more than 20 years ago are still working 😉.

### Step 5.: Prepare DC for OS-installation

* **Note:** Each time the Linux-OS write data on DC, it calculate the free remaining space. Use/partition your DC using 
full GiB & let some empty GiB at end of DC 😉. Having fractional amount of GiB, MiG or KiB at end of DC, the OS must 
calculate each time small fractions/numbers of space. Nonetheless, letting empty space at end of DC the system can 
write there data of deteriorate cluster, in addition, this method let exchange DC easily even if you decide to use 
another DC-manufacturer. 

1. Booth from Linux-Live-USB that have a DE like CachyOS, Mint, Garuda or whatever you like.

2. Assure that on your live-system following program are installed: `nvme-cli`, `gptfdisk` & `multipath-tools`. Further 
detailed explanation can be found [Here](https://github.com/Advantaged/4Kn-Formatting).

3. Detect DC-name through/with commands `lsblk`.

4. Convert, if it is possible your DC to "4Kn" LBA/LBS, this mean using clusters of 4-Kib (4096 byte) instead of very 
old 512 byte. Detailed information, explanation & suggestion can be found 
[Here](https://github.com/Advantaged/4Kn-Formatting), anyway…:

4.1. Detect the cluster dimension & if your DC  can be converted to "4Kn" trhough/with following command:

	`sudo nvme id-ns /dev/nvme0n1 -H | grep LBA`

4.2. If `Good` is in use & `Better` can be chooses, than format the controller to 4-KiB with following command:

	`sudo nvme format /dev/nvme0n1 -l 1`

* When the system commit the concluded "formatting", use command under pint "4.1." to countercheck the results.

5. Detect all particulars of your DC through/with command `fdisk -l /dev/nvme0n1`.

6. Just on the first line you will find, the total amount of bytes, at this stage divide the total bytes by 3 time 
1024, e.g. `2000398934016/1024/1024/1024 = 1863 GiB`. Plane now how to partition your DC, e.g. **"4 GiB for EFI"**, 
**"1850 GiB for OS"** & let the remain space **empty**. Partitions-table-codes can be found 
[Here](https://github.com/Advantaged/4Kn-Formatting/partition-codes.md). My recommandation is to use partition-code 
`EF00` for EFI & patirion-code `BF00` for the OS if you choose `zfs` or `btrfs` as file-system for the OS.

* **Notes:**
	* Use a program like `cgdisk`, `cfdisk` or `gdisk` with `sudo` for partitioning. First reset the 
partition-table making a new-one & than to make the new partitions like you want or recommended. These all are "A 
curses-based interactive text-mode program" 🟰 no commands in the CLI 😉.
	* Use `zram` instead of `swap` or `zswap`. CachyOS make it automatically by clicking "Don't use `Swap`", if your OS 
don't do it… install your OS without `swap` an add `zram` after installation, reboot & update of OS same. You can 
find all necessary information about `zram` [Here](https://github.com/Advantaged/ZRAM).
	* Some OS-Installer are not able to format properly the `EFI`-partition, in this case you have to make it 
manually in the "CLI" like [Here](https://github.com/Advantaged/4Kn-Formatting) explained.
	* If you want to still use `ext4` as file system & have converted your DC to "4Kn", follow the link on the point 
above to force `ext4` to accept "4Kn". More modern FS like `zfs` & `btrfs` use "4-KiB" by default 😉.



✅ **Done** 👍 **& Enjoy** 😉.


.
