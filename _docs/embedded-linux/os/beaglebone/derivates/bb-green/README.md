---
template: article
title: Derivated OS Images for BeagleBone Boards
sitename: archives
---

## ubuntu-14.04-console-armhf-2014-08-13-apps-1400mb

### 14.04.0-v1 

[img](ubuntu-14.04-console-armhf-2014-08-13-apps-1400mb.bin.xz), [bmap](ubuntu-14.04-console-armhf-2014-08-13-apps-1400mb.bmap)

- base
	- ubuntu-14.04-console-armhf-2014-08-13.zip
- installed-packages
	- wireless-tools
	- iw
	- wpasupplicant
	- gawk
	- sysstat
	- jq
	- httpie
	- virt-what
	- socat
	- screen
	- xz-utils
	- vim
	- htop
	- build-essential
	- telnet
	- libbluetooth-dev


### 14.04.0-v2 

[img](ubuntu-14.04-console-armhf-2014-08-13-apps-1400mb-v2.bin.xz), [bmap](ubuntu-14.04-console-armhf-2014-08-13-apps-1400mb-v2.bmap)

- date
	- 2016/3/16
- base
	- ubuntu-14.04-console-armhf-2014-08-13-apps-1000mb.bin.xz
- installed packages (extras)
	- python3-pip
- installed python3 packages
	- psutils
- installed nodejs runtimes (via nodenv)
	- 4.4.0 (default)
	- 4.3.2
	- 5.7.1
- installed components
	- /opt/dotfiles (from https://github.com/yagamy4680/dotfiles)
	- /root/.nodenv
	- /root/.vim
- generated files
	- /opt/system

    ```
    OS_KERNEL       linux
    OS_DIST_NAME    ubuntu
    OS_DIST_CODENAME        trusty
    OS_ARCH x86_64
    OS_NAME linux-ubuntu-trusty
    ```


## ubuntu-14.04.3-console-armhf-2016-02-11

### 14.04.3-v1

(2016/4/26) Downloads: [img](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb.img.xz), [bmap](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb.bmap)

| property | value |
|---|---|
| base | [bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz](/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/) |
| kernel | as-is (4.1.17) |

- installed packages (extras)
	- python3-pip
- installed python3 packages
	- psutils
- installed nodejs runtimes (via nodenv)
	- 4.4.0 (default)
	- 4.3.2
	- 5.7.1
- installed components
	- `/opt/dotfiles` (from https://github.com/yagamy4680/dotfiles)
	- `/root/.nodenv`
	- `/root/.vim`
- generated files
	- /opt/system

    ```
    OS_KERNEL       linux
    OS_DIST_NAME    ubuntu
    OS_DIST_CODENAME        trusty
    OS_ARCH x86_64
    OS_NAME linux-ubuntu-trusty
    ```


### 14.04.3-v2 

(2016/07/07) Downloads: [img](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-v2.img.xz), [bmap](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-v2.bmap)

| property | value |
|---|---|
| base | [bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz](/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/) |
| kernel | as-is (4.1.17) |
| applicable | bb-black, bb-green |


- installed packages (extras)
	- parted
	- iotop
- installed nodejs runtimes (via nodenv)
	- **4.4.7** (default)
	- 4.4.0
	- 6.3.0
- installed components
	- /opt/dotfiles (from https://github.com/yagamy4680/dotfiles)
	- /root/.nodenv
	- /root/.vim


### 14.04.3-v3 

(2016/07/24) Downloads: [img](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-v3.img.xz), [bmap](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-v3.img.xz)

| property | value |
|---|---|
| base | [bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz](/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/) |
| kernel | as-is (4.1.17) |
| applicable | bb-black, bb-green |


- installed packages (extras)
	- N/A
- installed nodejs runtimes (via nodenv)
	- **4.4.7** (default)
	- 4.4.0
	- 6.3.0
- installed components
	- `/opt/dotfiles` (from https://github.com/yagamy4680/dotfiles)
	- `/root/.nodenv`
	- `/root/.vim`
- extras
	- change default timezone to `Asia/Tokyo`
	- `update-rc.d apache2 disable`
	- `update-rc.d udhcpd disable`
	- `update-rc.d pppd-dns disable`


### 14.04.3-v4 

(2016/11/08) Downloads: [img](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-v4.img.xz), [bmap](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-v4.bmap)

| property | value |
|---|---|
| base | [bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz](/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/) |
| kernel | as-is (4.1.17) |
| applicable | bb-black, bb-green |

- installed packages (extras)
	- N/A
- installed nodejs runtimes (via nodenv)
	- **4.4.7** (default)
	- 4.4.0
	- 6.3.0
- installed components
	- /opt/dotfiles (from https://github.com/yagamy4680/dotfiles)
	- /root/.nodenv
	- /root/.vim
- extras
	- `apt-get remove apache2 -y && apt-get purge apache2 -y`
	- `libudev-dev`
	- `libbluetooth-dev`
	- `bluetooth`
	- `bluez`


### 14.04.3-v5 

(2016/12/20) Downloads: [img](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-v5.img.xz), [bmap](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-v5.bmap) 

| property | value |
|---|---|
| base | [bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz](/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/) |
| kernel | as-is |
| applicable | bb-black, bb-green, bb-green-wireless (if applying [kernel](/embedded-linux/os/beaglebone/kernels/README.md) **4.4.39**) |

Based on [bbb-image-gen](https://github.com/yagamy4680/bbb-image-gen) (commit [6783cb79cf00e01162ad08e29dfb141f3c238914](https://github.com/yagamy4680/bbb-image-gen/commit/6783cb79cf00e01162ad08e29dfb141f3c238914)), build with following options:

```bash
export PATH="$PATH:/opt/yapps-env/tools/bmap-tools-3.2"
export PRE_BUILT_PACKAGES="bluez-5.32-src"
./gen-image "https://archives.t2t.io/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz"
```

- installed packages (extras)
	- **bluez 5.32**
	- libdbus-1-dev
	- libdbus-glib-1-dev
	- libglib2.0-dev
	- libical-dev
	- libreadline-dev
	- libudev-dev
	- libusb-dev
- installed nodejs runtimes (via nodenv)
	- **4.4.7** (default)
	- 4.7.0 (newly-added)
	- 6.9.2 (newly-added)
- installed components
	- /opt/dotfiles (from https://github.com/yagamy4680/dotfiles)
	- /root/.nodenv
	- /root/.vim
- extras
   - `apt-get remove apache2 -y && apt-get purge apache2 -y`


### 14.04.3-v6

(2016/12/29) Downloads: [img](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-v6.img.xz), [bmap](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-v6.bmap) 

| property | value |
|---|---|
| base | [bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz](/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/) |
| kernel | as-is |
| applicable | bb-black, bb-green, bb-green-wireless (if applying [kernel](/embedded-linux/os/beaglebone/kernels/README.md) **4.4.39**) |

Based on [bbb-image-gen](https://github.com/yagamy4680/bbb-image-gen) (commit [e8e88cb801b416b952e0c646fca1d38681b306f5](https://github.com/yagamy4680/bbb-image-gen/commit/e8e88cb801b416b952e0c646fca1d38681b306f5)), build with following options:

```bash
export PATH="$PATH:/opt/yapps-env/tools/bmap-tools-3.2"
export PRE_BUILT_PACKAGES="bluez-5.32-src,fswebcam-src"
export BASE_IMAGE_URL="https://archives.t2t.io/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz"
./gen-image ${BASE_IMAGE_URL}
```

- installed packages (extras)
	- **bluez 5.32**
	- (bluez) libdbus-1-dev
	- (bluez) libdbus-glib-1-dev
	- (bluez) libglib2.0-dev
	- (bluez) libical-dev
	- (bluez) libreadline-dev
	- (bluez) libudev-dev
	- (bluez) libusb-dev
	- **fswebcam**
	- (fswebca) libgd2-xpm-dev
	- (fswebca) libjpeg-dev
	- (fswebca) libpng-dev
	- (fswebca) libfreetype6-dev
	- (misc.) dnsmasq 
	- (misc.) isc-dhcp-server 
	- (misc.) hostapd
- installed nodejs runtimes (via nodenv)
	- **4.4.7** (default)
	- 4.7.0
	- 6.9.2
- installed components
	- /opt/dotfiles (from https://github.com/yagamy4680/dotfiles)
	- /root/.nodenv
	- /root/.vim
- extras
   - `apt-get remove apache2 -y && apt-get purge apache2 -y`
   - `apt-get remove udhcpd -y && apt-get purge udhcpd -y`
   - `update-rc.d dnsmasq disable`
   - `update-rc.d isc-dhcp-server disable`


## References

```text
2015-10-09 - v4.1.10-ti-r21 kernel
2015-09-11 - v4.1.6-ti-r15 kernel
2015-08-17 - v4.1.5-ti-r10 kernel
2016-02-11 - v4.1.17-ti-rt-r47 kernel
```
