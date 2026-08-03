# ubuntu-server-software-raid

## Case I. Bootable RAID array.

1. You need to mark both disks as boot devices.
 - For the first, select it, hit enter, select the option to make it a boot device.
 - For the second, select it, hit enter, select the option to make it secondary boot device.

2. You need to create empty, unmounted partitions on both disks.

3. You hit the option to create a software RAID array, you select RAID level and ***pick the empty partitions***.

## Case II. Non Bootable RAID array.

If you plan just to make a RAID array just for any other case than booting from it, which it may be a more rare scenario than making a bootable raid array as said on `Case 1`, then things are more straight forward.

1. Hit the option to create a software RAID array.
2. Select the RAID level and then the disks accordingly.
