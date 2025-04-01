# Shrink-WD-partition.md

## Shrink Windows Partition
To shrink a partition in Windows using built-in tools, you can use either Disk Management or DiskPart. Disk Management 
is a graphical interface tool that allows you to easily manage disk volumes, including shrinking partitions. Here’s how 
to use Disk Management:

### 1. Solution: Disk Management

1. Right-click on the Windows icon and select "Disk Management."
2. **Right-click on the partition you want to shrink and select "Shrink Volume."**
3. Enter the amount of space you want to shrink in MB and click "Shrink."

### 2. Solution: DiskPart

DiskPart is a command-line utility that offers similar functionality but requires manual entry of commands. Here’s 
how to use DiskPart:

1. Press the Windows logo key + R, type "diskpart," and press Enter.
2. At the DISKPART prompt, enter `list volume` to see the list of volumes.
3. Select the volume you want to shrink by entering `select volume X` (replace X with the volume number).
4. Enter shrink `[desired=] [minimum=]` to shrink the volume by the specified amount in MB.

* Both tools can only shrink NTFS partitions and cannot shrink OEM partitions, ESP partitions, Recovery partitions, 
offline volumes, and non-NTFS partitions.

* Disk Management is generally easier to use for most users, while DiskPart offers more flexibility for advanced users 
who prefer command-line interfaces.

* EaseUS Partition Master is also mentioned as a versatile tool that can handle more complex scenarios, such as 
shrinking partitions with unmovable files or corrupted file systems, but it is not a built-in Windows tool.
