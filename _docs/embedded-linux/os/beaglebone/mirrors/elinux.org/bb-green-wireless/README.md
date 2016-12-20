---
template: article
title: Kernels
sitename: archives
---

Mirror from https://rcn-ee.com/rootfs/bb.org/testing/


###  bone-debian-8.6-seeed-iot-armhf-2016-12-18-4gb 

- Origin: [2016-12-18 / seeed-iot](https://rcn-ee.com/rootfs/bb.org/testing/2016-12-18/seeed-iot/)
- Mirror: [img.xz](bone-debian-8.6-seeed-iot-armhf-2016-12-18-4gb.img.xz), [bmap](bone-debian-8.6-seeed-iot-armhf-2016-12-18-4gb.bmap)

```text
bone-debian-8.6-seeed-iot-armhf-2016-12-18-4gb.bmap
bone-debian-8.6-seeed-iot-armhf-2016-12-18-4gb.img.xz

root@beaglebone:~# uname -a
Linux beaglebone 4.4.39-ti-r75 #1 SMP Thu Dec 15 22:16:11 UTC 2016 armv7l GNU/Linux

root@beaglebone:~# lsb_release -a
No LSB modules are available.
Distributor ID:	Debian
Description:	Debian GNU/Linux 8.6 (jessie)
Release:	8.6
Codename:	jessie

# hcitool --version
hcitool: unrecognized option '--version'
hcitool - HCI Tool ver 4.101


root@beaglebone:~# hcitool
hcitool - HCI Tool ver 5.23
Usage:

root@beaglebone:/home/debian# df -h
df -h
Filesystem      Size  Used Avail Use% Mounted on
udev             10M     0   10M   0% /dev
tmpfs            98M  2.8M   95M   3% /run
/dev/mmcblk0p1  3.3G  1.7G  1.4G  54% /
tmpfs           245M     0  245M   0% /dev/shm
tmpfs           5.0M     0  5.0M   0% /run/lock
tmpfs           245M     0  245M   0% /sys/fs/cgroup
tmpfs            49M     0   49M   0% /run/user/1000
root@beaglebone:/home/debian#
root@beaglebone:/home/debian#
root@beaglebone:/home/debian# du -s -m /*
du -s -m /*
6   /bin
25  /boot
0   /dev
5   /etc
1   /home
1   /ID.txt
155 /lib
1   /log
1   /lost+found
1   /media
1   /mnt
1   /nfs-uEnv.txt
109 /opt
du: cannot access ‘/proc/5385/task/5385/fd/3’: No such file or directory
du: cannot access ‘/proc/5385/task/5385/fdinfo/3’: No such file or directory
du: cannot access ‘/proc/5385/fd/3’: No such file or directory
du: cannot access ‘/proc/5385/fdinfo/3’: No such file or directory
0   /proc
41  /root
3   /run
6   /sbin
1   /srv
0   /sys
1   /tmp
1   /uEnv.txt
1124    /usr
193 /var


root@beaglebone:~# socat -d -d - file:/dev/ttyO4,b38400,nonblock,raw,echo=0,crnl
2016/12/19 13:47:07 socat[5222] N reading from and writing to stdio
2016/12/19 13:47:07 socat[5222] N opening character device "/dev/ttyO4" for reading and writing
2016/12/19 13:47:07 socat[5222] N starting data transfer loop with FDs [0,1] and [5,5]
!	0000	S	___	heartbeat	enter	.
^C2016/12/19 13:47:11 socat[5222] N socat_signal(): handling signal 2
2016/12/19 13:47:11 socat[5222] N exiting on signal 2
2016/12/19 13:47:11 socat[5222] N socat_signal(): finishing signal 2
2016/12/19 13:47:11 socat[5222] N exit(130)


root@beaglebone:~# socat -d -d - file:/dev/ttyO1,b57600,nonblock,raw,echo=0,crnl
2016/12/19 13:47:14 socat[5223] N reading from and writing to stdio
2016/12/19 13:47:14 socat[5223] N opening character device "/dev/ttyO1" for reading and writing
2016/12/19 13:47:14 socat[5223] N starting data transfer loop with FDs [0,1] and [5,5]
T22.4
H52.3
^C2016/12/19 13:47:19 socat[5223] N socat_signal(): handling signal 2
2016/12/19 13:47:19 socat[5223] N exiting on signal 2
2016/12/19 13:47:19 socat[5223] N socat_signal(): finishing signal 2
2016/12/19 13:47:19 socat[5223] N exit(130)


root@beaglebone:~# hcitool lescan
LE Scan ...
F4:21:56:15:32:20 FOOP_0.5.4_155621F4
C7:25:50:D3:0B:DC FOOP_0.5.4_D35025C7
C7:25:50:D3:0B:DC (unknown)
C5:93:B6:66:94:DA FOOP_0.5.4_66B693C5
C5:93:B6:66:94:DA (unknown)
F4:21:56:15:32:20 FOOP_0.5.4_155621F4
D0:4F:7E:17:62:1C (unknown)
D0:4F:7E:17:62:1C (unknown)
D2:32:DE:13:E2:56 FOOP_0.5.4_13DE32D2
D2:32:DE:13:E2:56 (unknown)
FD:B5:52:E9:8C:35 FOOP_0.5.4_E952B5FD
E3:F6:BE:93:BD:B7 (unknown)
E3:F6:BE:93:BD:B7 Prodigio_E3F6BE93BDB7


^Croot@beaglebone:~#
root@beaglebone:~# ps aux | grep hci
root      2912  0.0  0.0      0     0 ?        S<   13:43   0:00 [hci0]
root      2913  0.0  0.0      0     0 ?        S<   13:43   0:00 [hci0]
root      2995  0.0  0.1   1588   644 ?        S    13:43   0:00 /usr/bin/hciattach /dev/ttyS3 texas 300000
root      5226  0.0  0.3   3680  1632 pts/0    S+   13:47   0:00 grep hci
```

Kernel extraction: [bone-debian-8.6-seeed-iot-armhf-2016-12-18-kernel-4.4.39-extraction.tar.gz](bone-debian-8.6-seeed-iot-armhf-2016-12-18-kernel-4.4.39-extraction.tar.gz).