# Install minibian (https://sourceforge.net/projects/minibian/)

Identify the SD card

    diskutil list

	/dev/disk2 (internal, physical):
    #:                       TYPE NAME                    SIZE       IDENTIFIER
    0:     FDisk_partition_scheme                        *15.9 GB    disk2
    1:             Windows_FAT_32 boot                    62.9 MB    disk2s1
    2:                      Linux                         15.9 GB    disk2s2

Unmount

	diskutil unmountDisk /dev/disk2

	Unmount of all volumes on disk2 was successful

Copy minibian image on the SD card

	sudo dd bs=1m if=2015-11-12-jessie-minibian.img of=/dev/disk2

Eject the card.