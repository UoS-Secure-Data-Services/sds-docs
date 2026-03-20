# Helpful Hints

If there's something you're looking for here, and it's not here, chances are it should be so get in touch and we'll add it.

## Can't see the disk you've added in a Windows machine?

If you're wondering why you can't see the disk you've added to a windows machine, you'll need to follow these instructions, they won't appear automatically

+ [Preparing a new disk in Windows](https://learn.microsoft.com/en-us/windows-server/storage/disk-management/initialize-new-disks)

Alternatively, you might be moving a disk from one Windows machine to another

+ [Moving a disk between Windows machines in Ronin](https://blog.ronin.cloud/lifes-too-short-to-troubleshoot-windows/)

## Can't see the disk you've added in a Linux machine?

Your disk will be in the directory **/mnt/sdX** where **X** should be **d** for the first additional disk (incrementing alphabetically for each additional disk), if you specified it at machine creation. 

If not, you'll have to reboot the machine then find the disk in the /dev/ directory and create an /etc/fstab entry using sudo before mounting. 
