# Introduction

- This project is based on: https://github.com/foss-for-synopsys-dwc-arc-processors/buildroot/archive/arc-2015.08-3.tar.gz

## Build .img file
> make snps_axs101_defconfig

> make

sdcard.img will be prepared in output/images

## Format the SD card
> Download and install SDFormatter from  https://www.sdcard.org/downloads/formatter_4/

> Run SDFormatter, Choose Option->FORMAT SIZE ADJUSTMENT [ON]

> Click Format

## Install Linux into SD card
> Download and install "Win32 Disk Imager" https://sourceforge.net/projects/win32diskimager/

> Run "Win32 Disk Imager" and choose sdcard.img

> Click Write

## Resize file system
> fdisk /dev/mmcblk0

> (d,2,n,p,2,enter,enter,w)

> reboot the system

> resize2fs /dev/mmcblk0p2 

