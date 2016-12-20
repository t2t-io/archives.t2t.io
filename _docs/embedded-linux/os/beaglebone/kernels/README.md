---
template: article
title: Kernels
sitename: archives
---

Here are list of kernels from different sources:

1. built from scratch
2. extract from prebuilt os image released by community (e.g. http://elinux.org)
3. extract from os embedded on the emmc of shipped boards


## Kernels from Prebuilt Image

| version | archive | source |
|---|---|---|
| 4.4.6 | [ubuntu-14.04.3-console-armhf-2016-04-07-kernel-4.4.6.tar.gz](ubuntu-14.04.3-console-armhf-2016-04-07-kernel-4.4.6.tar.gz) | [elinux](https://rcn-ee.online/rootfs/2016-04-07/microsd/bone-ubuntu-16.04-console-armhf-2016-04-07-2gb.img.xz) |
| 4.4.12 | [bone-ubuntu-16.04-console-armhf-2016-06-09-2gb-kernel-4.4.12.tar.gz](bone-ubuntu-16.04-console-armhf-2016-06-09-2gb-kernel-4.4.12.tar.gz) | [elinux](https://rcn-ee.online/rootfs/2016-06-09/microsd/) |
| 4.4.39 | [bone-debian-8.6-seeed-iot-armhf-2016-12-18-kernel-4.4.39.tar.gz](bone-debian-8.6-seeed-iot-armhf-2016-12-18-kernel-4.4.39.tar.gz) | [elinux/testing](https://rcn-ee.com/rootfs/bb.org/testing/) ([local mirror](/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green-wireless/README.md)) |


## Kernels from EMMC Dumps

### bbgw-emmc-debian-20160527

Please download it from [bbgw-emmc-debian-20160527-kernel-4.4.9-extraction.tar.gz](bbgw-emmc-debian-20160527-kernel-4.4.9-extraction.tar.gz).

```text
root@beaglebone:/home/debian# uname -a
Linux beaglebone 4.4.9-ti-r25 #1 SMP Thu May 5 23:08:13 UTC 2016 armv7l GNU/Linux


root@beaglebone:/home/debian# lsb_release -a
No LSB modules are available.
Distributor ID:	Debian
Description:	Debian GNU/Linux 8.4 (jessie)
Release:	8.4
Codename:	jessie


root@beaglebone:/home/debian# ls -al /boot
total 15712
drwxr-xr-x  4 root root    4096 Dec 17 08:23 .
drwxr-xr-x 21 root root    4096 Jan  1  2000 ..
-rw-r--r--  1 root root  143853 May  5  2016 config-4.4.9-ti-r25
drwxr-xr-x  3 root root    4096 May 27  2016 dtbs
-rw-r--r--  1 root root 4767302 Dec 17 08:23 initrd.img-4.4.9-ti-r25
-rw-r--r--  1 root root     492 May 27  2016 SOC.sh
-rw-r--r--  1 root root 3313638 May  5  2016 System.map-4.4.9-ti-r25
drwxr-xr-x  2 root root    4096 May 27  2016 uboot
-rw-r--r--  1 root root    1185 Jan  1  2000 uEnv.txt
-rwxr-xr-x  1 root root 7833256 May  5  2016 vmlinuz-4.4.9-ti-r25


root@beaglebone:/home/debian# cat /ID.txt
BeagleBoard.org Debian Image 2016-05-27
```

