# buildroot-arc-ext4fs

- arc-2015.08-3.tar.gz: https://github.com/foss-for-synopsys-dwc-arc-processors/buildroot/archive/arc-2015.08-3.tar.gz
- buildroot-ext4fs: buildroot-arc-2015.08-3

## resize file system
> fdisk /dev/mmcblk0

> (d,2,n,p,2,enter,enter,w)

> reboot the system

> resize2fs /dev/mmcblk0p2 

