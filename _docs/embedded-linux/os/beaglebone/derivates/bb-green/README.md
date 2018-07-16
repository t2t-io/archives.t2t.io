---
template: article
title: Derivated OS Images for BeagleBone Boards
sitename: archives
---

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [ubuntu-14.04-console-armhf-2014-08-13-apps-1400mb](#ubuntu-1404-console-armhf-2014-08-13-apps-1400mb)
  - [14.04.0-v1](#14040-v1)
  - [14.04.0-v2](#14040-v2)
- [ubuntu-14.04.3-console-armhf-2016-02-11](#ubuntu-14043-console-armhf-2016-02-11)
  - [14.04.3-v1](#14043-v1)
  - [14.04.3-v2](#14043-v2)
  - [14.04.3-v3](#14043-v3)
  - [14.04.3-v4](#14043-v4)
  - [14.04.3-v5](#14043-v5)
  - [14.04.3-v6](#14043-v6)
  - [14.04.3-v7](#14043-v7)
  - [14.04.3-r8](#14043-r8)
  - [14.04.3-r9](#14043-r9)
  - [14.04.3-r10](#14043-r10)
  - [14.04.3-r11](#14043-r11)
  - [14.04.3-r14](#14043-r14)
  - [14.04.3-r15](#14043-r15)
- [References](#references)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

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


### 14.04.3-v7

(2017/01/02) Downloads: [img](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-v7.img.xz), [bmap](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-v7.bmap) 

| property | value |
|---|---|
| base | [bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz](/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/) |
| kernel | as-is |
| applicable | bb-black, bb-green, bb-green-wireless (if applying [kernel](/embedded-linux/os/beaglebone/kernels/README.md) **4.4.39**) |

Based on [bbb-image-gen](https://github.com/yagamy4680/bbb-image-gen) (commit [0ff3bda07b796e22f645f72a433ae2e7887f1292](https://github.com/yagamy4680/bbb-image-gen/commit/0ff3bda07b796e22f645f72a433ae2e7887f1292)), build with following options:

```bash
export PATH="$PATH:/opt/yapps-env/tools/bmap-tools-3.2"
export PRE_BUILT_PACKAGES="bluez-5.32-src,fswebcam-src"
export BASE_IMAGE_URL="https://archives.t2t.io/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz"
./gen-image ${BASE_IMAGE_URL}
```

Comparing to v6, here are changes:

- `apt-get install ntp`
- `update-rc.d ntp disable`


### 14.04.3-r8

(2017/01/22) Downloads: [img](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-r8.img.xz), [bmap](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-r8.bmap) 

| property | value |
|---|---|
| base | [bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz](/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/) |
| kernel | as-is |
| applicable | bb-black, bb-green, bb-green-wireless (if applying [kernel](/embedded-linux/os/beaglebone/kernels/README.md) **4.4.39**) |

Based on [bbb-image-gen](https://github.com/yagamy4680/bbb-image-gen) (commit [0ff3bda07b796e22f645f72a433ae2e7887f1292](https://github.com/yagamy4680/bbb-image-gen/commit/0ff3bda07b796e22f645f72a433ae2e7887f1292)), build with following options:

```bash
export PATH="$PATH:/opt/yapps-env/tools/bmap-tools-3.2"
export PRE_BUILT_PACKAGES="bluez-5.32-src,fswebcam-src"
export BASE_IMAGE_URL="https://archives.t2t.io/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz"
./gen-image ${BASE_IMAGE_URL}
```

Comparing to v7, here are changes:

- install [httpie](https://httpie.org/) via `pip` instead of `apt-get`
- remove [dnsmasq](http://www.thekelleys.org.uk/dnsmasq/doc.html) and [isc-dhcp-server](https://www.isc.org/downloads/dhcp/) from installation list
- move [hostapd](http://w1.fi/hostapd/) to `apt-packages.conf`
- apt-get install:
  - `libcurl4-openssl-dev`
  - `libsqlite3-dev`
  - `sqlite3`
  - `python-dev`
  - `cmake`
- pip install:
  - `socketIO_client`
  - `netifaces`
  - `colorama`


### 14.04.3-r9

(2017/03/24) Downloads: [img](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-r9.img.xz), [bmap](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-r9.bmap), and [sqfs](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-r9.sqsh) 

| property | value |
|---|---|
| base | [bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz](/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/) |
| kernel | as-is |
| applicable | bb-black, bb-green, bb-green-wireless (if applying [kernel](/embedded-linux/os/beaglebone/kernels/README.md) **4.4.39**) |

Based on [bbb-image-gen](https://github.com/yagamy4680/bbb-image-gen) (commit [37d8a3c231e28d94200705fabaff3c9165482907](https://github.com/yagamy4680/bbb-image-gen/commit/37d8a3c231e28d94200705fabaff3c9165482907)), build with following options:

```bash
export PATH="$PATH:/opt/yapps-env/tools/bmap-tools-3.2"
export PRE_BUILT_PACKAGES="bluez-5.32-src,fswebcam-src"
export BASE_IMAGE_URL="https://archives.t2t.io/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz"
./gen-image ${BASE_IMAGE_URL}
```

Comparing to r8, here are changes:

- install `gatttool` from bluez to system directory
- debian package upgrades

| name | r8.txt | current.txt |
|---|---|---|
| bind9-host | `1:9.9.5.dfsg-3ubuntu0.11` | `1:9.9.5.dfsg-3ubuntu0.13` |
| dnsutils | `1:9.9.5.dfsg-3ubuntu0.11` | `1:9.9.5.dfsg-3ubuntu0.13` |
| krb5-multidev | `1.12+dfsg-2ubuntu5.2` | `1.12+dfsg-2ubuntu5.3` |
| libarchive13:armhf | `3.1.2-7ubuntu2.3` | `3.1.2-7ubuntu2.4` |
| libbind9-90 | `1:9.9.5.dfsg-3ubuntu0.11` | `1:9.9.5.dfsg-3ubuntu0.13` |
| libdns100 | `1:9.9.5.dfsg-3ubuntu0.11` | `1:9.9.5.dfsg-3ubuntu0.13` |
| libfreetype6:armhf | `2.5.2-1ubuntu2.5` | `2.5.2-1ubuntu2.6` |
| libfreetype6-dev | `2.5.2-1ubuntu2.5` | `2.5.2-1ubuntu2.6` |
| libgd-dev:armhf | `2.1.0-3ubuntu0.5` | `2.1.0-3ubuntu0.6` |
| libgd2-xpm-dev | `2.1.0-3ubuntu0.5` | `2.1.0-3ubuntu0.6` |
| libgd3:armhf | `2.1.0-3ubuntu0.5` | `2.1.0-3ubuntu0.6` |
| libgnutls-dev | `2.12.23-12ubuntu2.5` | `2.12.23-12ubuntu2.7` |
| libgnutls-openssl27:armhf | `2.12.23-12ubuntu2.5` | `2.12.23-12ubuntu2.7` |
| libgnutls26:armhf | `2.12.23-12ubuntu2.5` | `2.12.23-12ubuntu2.7` |
| libgnutlsxx27:armhf | `2.12.23-12ubuntu2.5` | `2.12.23-12ubuntu2.7` |
| libgssapi-krb5-2:armhf | `1.12+dfsg-2ubuntu5.2` | `1.12+dfsg-2ubuntu5.3` |
| libgssrpc4:armhf | `1.12+dfsg-2ubuntu5.2` | `1.12+dfsg-2ubuntu5.3` |
| libisc95 | `1:9.9.5.dfsg-3ubuntu0.11` | `1:9.9.5.dfsg-3ubuntu0.13` |
| libisccfg90 | `1:9.9.5.dfsg-3ubuntu0.11` | `1:9.9.5.dfsg-3ubuntu0.13` |
| libk5crypto3:armhf | `1.12+dfsg-2ubuntu5.2` | `1.12+dfsg-2ubuntu5.3` |
| libkadm5clnt-mit9:armhf | `1.12+dfsg-2ubuntu5.2` | `1.12+dfsg-2ubuntu5.3` |
| libkadm5srv-mit9:armhf | `1.12+dfsg-2ubuntu5.2` | `1.12+dfsg-2ubuntu5.3` |
| libkdb5-7:armhf | `1.12+dfsg-2ubuntu5.2` | `1.12+dfsg-2ubuntu5.3` |
| libkrb5-3:armhf | `1.12+dfsg-2ubuntu5.2` | `1.12+dfsg-2ubuntu5.3` |
| libkrb5-dev | `1.12+dfsg-2ubuntu5.2` | `1.12+dfsg-2ubuntu5.3` |
| libkrb5support0:armhf | `1.12+dfsg-2ubuntu5.2` | `1.12+dfsg-2ubuntu5.3` |
| liblwres90 | `1:9.9.5.dfsg-3ubuntu0.11` | `1:9.9.5.dfsg-3ubuntu0.13` |
| libnettle4:armhf | `2.7.1-1ubuntu0.1` | `2.7.1-1ubuntu0.2` |
| libssl-dev:armhf | `1.0.1f-1ubuntu2.21` | `1.0.1f-1ubuntu2.22` |
| libssl-doc | `1.0.1f-1ubuntu2.21` | `1.0.1f-1ubuntu2.22` |
| libssl1.0.0:armhf | `1.0.1f-1ubuntu2.21` | `1.0.1f-1ubuntu2.22` |
| libtiff5:armhf | `4.0.3-7ubuntu0.4` | `4.0.3-7ubuntu0.6` |
| libtiff5-dev:armhf | `4.0.3-7ubuntu0.4` | `4.0.3-7ubuntu0.6` |
| libtiffxx5:armhf | `4.0.3-7ubuntu0.4` | `4.0.3-7ubuntu0.6` |
| libudev-dev | `204-5ubuntu20.20` | `204-5ubuntu20.24` |
| libudev1:armhf | `204-5ubuntu20.20` | `204-5ubuntu20.24` |
| libxpm-dev:armhf | `1:3.5.10-1` | `1:3.5.10-1ubuntu0.1` |
| libxpm4:armhf | `1:3.5.10-1` | `1:3.5.10-1ubuntu0.1` |
| udev | `204-5ubuntu20.20` | `204-5ubuntu20.24` |


### 14.04.3-r10

(2017/04/01) Downloads: [img](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-r10.img.xz), [bmap](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-r10.bmap). README: [markdown](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-r10.md)

| property | value |
|---|---|
| base | [bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz](/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/) |
| kernel | as-is |
| applicable | bb-black, bb-green, bb-green-wireless (if applying [kernel](/embedded-linux/os/beaglebone/kernels/README.md) **4.4.39**) |

Based on [bbb-image-gen](https://github.com/yagamy4680/bbb-image-gen) (commit [a3a9ce5d1ed0209dd24e1d596f35e8d987c88a0d](https://github.com/yagamy4680/bbb-image-gen/commit/a3a9ce5d1ed0209dd24e1d596f35e8d987c88a0d)), build with following options:

```bash
export PATH="$PATH:/opt/yapps-env/tools/bmap-tools-3.2"
export PRE_BUILT_PACKAGES="bluez-5.32-src,fswebcam-src"
export BASE_IMAGE_URL="https://archives.t2t.io/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz"
./gen-image ${BASE_IMAGE_URL}
```

Comparing to previous version r9, here are major changes:

- Force the `setuptool` of python2 and python3 are upgraded
- Extra python2 packages
  - inflection
- Extra python3 packages
  - pybars3
  - ruamel.yaml
  - colorama
  - socketIO_client
  - netifaces
  - inflection
- dotfiles
  - upgrade nodejs 4.7.0 to 4.8.1
  - upgrade nodejs 6.9.2 to 6.10.1
  - install nodejs 7.8.1 for experiments
  - update all git submodules


### 14.04.3-r11

Based on [bbb-image-gen](https://github.com/yagamy4680/bbb-image-gen) (commit [82142fc029e8374b55a630fe823a6514fc7108f6](https://github.com/yagamy4680/bbb-image-gen/commit/82142fc029e8374b55a630fe823a6514fc7108f6)), build with following options:

```bash
export PATH="$PATH:/opt/yapps-env/tools/bmap-tools-3.2"
export PRE_BUILT_PACKAGES="bluez-5.32-src,fswebcam-src"
export BASE_IMAGE_URL="https://archives.t2t.io/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz"
./gen-image ${BASE_IMAGE_URL}
```

Comparing to previous version r10, here are major changes:

- Extra system packages:
  - `avahi-utils`
- [dotfiles](https://github.com/yagamy4680/dotfiles/commit/1da3825c7257ee78826705524717f7ba3fe7b7c9)
  - upgrade nodejs `4.8.1` to `4.8.7`
  - upgrade nodejs `6.10.1` to `6.12.3`
  - upgrade nodejs `7.8.0` to `8.9.4` (as next major nodejs runtime)
  - update all git submodules. ([2d858e088cbfe54c22a12cd7c88ed7f0e5ef981d](https://github.com/yagamy4680/dotfiles/commit/2d858e088cbfe54c22a12cd7c88ed7f0e5ef981d))

- debian package upgrades

| name | r10 | r11 |
|---|---|---|
| bind9-host | `1:9.9.5.dfsg-3ubuntu0.13` | `1:9.9.5.dfsg-3ubuntu0.16` |
| dnsutils | `1:9.9.5.dfsg-3ubuntu0.13` | `1:9.9.5.dfsg-3ubuntu0.16` |
| hostapd | `1:2.1-0ubuntu1.4` | `1:2.1-0ubuntu1.5` |
| libbind9-90 | `1:9.9.5.dfsg-3ubuntu0.13` | `1:9.9.5.dfsg-3ubuntu0.16` |
| libcurl3:armhf | `7.35.0-1ubuntu2.10` | `7.35.0-1ubuntu2.13` |
| libcurl4-openssl-dev:armhf | `7.35.0-1ubuntu2.10` | `7.35.0-1ubuntu2.13` |
| libdns100 | `1:9.9.5.dfsg-3ubuntu0.13` | `1:9.9.5.dfsg-3ubuntu0.16` |
| libexpat1:armhf | `2.1.0-4ubuntu1.3` | `2.1.0-4ubuntu1.4` |
| libexpat1-dev:armhf | `2.1.0-4ubuntu1.3` | `2.1.0-4ubuntu1.4` |
| libfreetype6:armhf | `2.5.2-1ubuntu2.6` | `2.5.2-1ubuntu2.8` |
| libfreetype6-dev | `2.5.2-1ubuntu2.6` | `2.5.2-1ubuntu2.8` |
| libgcrypt11:armhf | `1.5.3-2ubuntu4.4` | `1.5.3-2ubuntu4.5` |
| libgcrypt11-dev | `1.5.3-2ubuntu4.4` | `1.5.3-2ubuntu4.5` |
| libgd-dev:armhf | `2.1.0-3ubuntu0.6` | `2.1.0-3ubuntu0.8` |
| libgd2-xpm-dev | `2.1.0-3ubuntu0.6` | `2.1.0-3ubuntu0.8` |
| libgd3:armhf | `2.1.0-3ubuntu0.6` | `2.1.0-3ubuntu0.8` |
| libgnutls-dev | `2.12.23-12ubuntu2.7` | `2.12.23-12ubuntu2.8` |
| libgnutls-openssl27:armhf | `2.12.23-12ubuntu2.7` | `2.12.23-12ubuntu2.8` |
| libgnutls26:armhf | `2.12.23-12ubuntu2.7` | `2.12.23-12ubuntu2.8` |
| libgnutlsxx27:armhf | `2.12.23-12ubuntu2.7` | `2.12.23-12ubuntu2.8` |
| libidn11:armhf | `1.28-1ubuntu2.1` | `1.28-1ubuntu2.2` |
| libidn11-dev | `1.28-1ubuntu2.1` | `1.28-1ubuntu2.2` |
| libisc95 | `1:9.9.5.dfsg-3ubuntu0.13` | `1:9.9.5.dfsg-3ubuntu0.16` |
| libisccfg90 | `1:9.9.5.dfsg-3ubuntu0.13` | `1:9.9.5.dfsg-3ubuntu0.16` |
| libldap-2.4-2:armhf | `2.4.31-1+nmu2ubuntu8.3` | `2.4.31-1+nmu2ubuntu8.4` |
| libldap2-dev:armhf | `2.4.31-1+nmu2ubuntu8.3` | `2.4.31-1+nmu2ubuntu8.4` |
| liblwres90 | `1:9.9.5.dfsg-3ubuntu0.13` | `1:9.9.5.dfsg-3ubuntu0.16` |
| libpython2.7:armhf | `2.7.6-8ubuntu0.3` | `2.7.6-8ubuntu0.4` |
| libpython2.7-dev:armhf | `2.7.6-8ubuntu0.3` | `2.7.6-8ubuntu0.4` |
| libpython2.7-minimal:armhf | `2.7.6-8ubuntu0.3` | `2.7.6-8ubuntu0.4` |
| libpython2.7-stdlib:armhf | `2.7.6-8ubuntu0.3` | `2.7.6-8ubuntu0.4` |
| libpython3.4:armhf | `3.4.3-1ubuntu1~14.04.5` | `3.4.3-1ubuntu1~14.04.6` |
| libpython3.4-dev:armhf | `3.4.3-1ubuntu1~14.04.5` | `3.4.3-1ubuntu1~14.04.6` |
| libpython3.4-minimal:armhf | `3.4.3-1ubuntu1~14.04.5` | `3.4.3-1ubuntu1~14.04.6` |
| libpython3.4-stdlib:armhf | `3.4.3-1ubuntu1~14.04.5` | `3.4.3-1ubuntu1~14.04.6` |
| librtmp-dev | `2.4+20121230.gitdf6c518-1` | `2.4+20121230.gitdf6c518-1ubuntu0.1` |
| librtmp0:armhf | `2.4+20121230.gitdf6c518-1` | `2.4+20121230.gitdf6c518-1ubuntu0.1` |
| libssl-dev:armhf | `1.0.1f-1ubuntu2.22` | `1.0.1f-1ubuntu2.23` |
| libssl-doc | `1.0.1f-1ubuntu2.22` | `1.0.1f-1ubuntu2.23` |
| libssl1.0.0:armhf | `1.0.1f-1ubuntu2.22` | `1.0.1f-1ubuntu2.23` |
| libtasn1-6:armhf | `3.4-3ubuntu0.4` | `3.4-3ubuntu0.5` |
| libtasn1-6-dev | `3.4-3ubuntu0.4` | `3.4-3ubuntu0.5` |
| libtiff5:armhf | `4.0.3-7ubuntu0.6` | `4.0.3-7ubuntu0.7` |
| libtiff5-dev:armhf | `4.0.3-7ubuntu0.6` | `4.0.3-7ubuntu0.7` |
| libtiffxx5:armhf | `4.0.3-7ubuntu0.6` | `4.0.3-7ubuntu0.7` |
| libudev-dev | `204-5ubuntu20.24` | `204-5ubuntu20.25` |
| libudev1:armhf | `204-5ubuntu20.24` | `204-5ubuntu20.25` |
| ntp | `1:4.2.6.p5+dfsg-3ubuntu2.14.04.10` | `1:4.2.6.p5+dfsg-3ubuntu2.14.04.12` |
| python2.7 | `2.7.6-8ubuntu0.3` | `2.7.6-8ubuntu0.4` |
| python2.7-dev | `2.7.6-8ubuntu0.3` | `2.7.6-8ubuntu0.4` |
| python2.7-minimal | `2.7.6-8ubuntu0.3` | `2.7.6-8ubuntu0.4` |
| python3.4 | `3.4.3-1ubuntu1~14.04.5` | `3.4.3-1ubuntu1~14.04.6` |
| python3.4-dev | `3.4.3-1ubuntu1~14.04.5` | `3.4.3-1ubuntu1~14.04.6` |
| python3.4-minimal | `3.4.3-1ubuntu1~14.04.5` | `3.4.3-1ubuntu1~14.04.6` |
| udev | `204-5ubuntu20.24` | `204-5ubuntu20.25` |
| wpasupplicant | `2.1-0ubuntu1.4` | `2.1-0ubuntu1.5` |
| xtrans-dev | `1.3.5-1~ubuntu14.04.1` | `1.3.5-1~ubuntu14.04.2` |


### 14.04.3-r14

(2018/03/27) Downloads: [img](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-r14.img.xz), [bmap](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-r14.bmap).

| property | value |
|---|---|
| base | [bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz](/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/) |
| kernel | as-is |
| applicable | bb-black, bb-green, bb-green-wireless (if applying [kernel](/embedded-linux/os/beaglebone/kernels/README.md) **4.4.39**) |

Based on [bbb-image-gen](https://github.com/yagamy4680/bbb-image-gen) (commit [82142fc029e8374b55a630fe823a6514fc7108f6](https://github.com/yagamy4680/bbb-image-gen/commit/82142fc029e8374b55a630fe823a6514fc7108f6)), build with following options:

```bash
export PATH="$PATH:/opt/yapps-env/tools/bmap-tools-3.2"
export BASE_IMAGE_URL="https://archives.t2t.io/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz"
export PRE_BUILT_PACKAGES="bluez-5.32-src,fswebcam-src,eprog-0.7.7-github,socat-1.7.3.2-src"
./gen-image ${BASE_IMAGE_URL}
```

Comparing to previous version r11, here are major changes:

- Extra debian packages
  - `squashfs-tools`
  - `pv`
  - `dnsmasq`
- Extra source packages
  - [eeprog](https://github.com/jsarenik/eeprog), 0.7.6
  - [socat](http://www.dest-unreach.org/socat), upgraded from 1.7.2.3 to 1.7.3.2
- Extra python2 packages
  - `socketIO_client_nexus`
- Extra python3 packages
  - `socketIO_client_nexus`
  - `shyaml`
- dotfiles
  - upgrade nodejs `4.8.1` to `4.8.7`
  - upgrade nodejs `6.10.1` to `6.12.3`
  - install nodejs `8.9.4` for experiments
  - update all git submodules

| type | name | r11 | r14 |
|---|---|---|---|
| debian | bind9-host | `1:9.9.5.dfsg-3ubuntu0.16` | `1:9.9.5.dfsg-3ubuntu0.17` |
| debian | dnsmasq | `2.68-1ubuntu0.1` | `2.68-1ubuntu0.2` |
| debian | dnsmasq-base | `2.68-1ubuntu0.1` | `2.68-1ubuntu0.2` |
| debian | dnsutils | `1:9.9.5.dfsg-3ubuntu0.16` | `1:9.9.5.dfsg-3ubuntu0.17` |
| debian | libbind9-90 | `1:9.9.5.dfsg-3ubuntu0.16` | `1:9.9.5.dfsg-3ubuntu0.17` |
| debian | libcurl3 | `7.35.0-1ubuntu2.13` | `7.35.0-1ubuntu2.15` |
| debian | libcurl4-openssl-dev | `7.35.0-1ubuntu2.13` | `7.35.0-1ubuntu2.15` |
| debian | libdns100 | `1:9.9.5.dfsg-3ubuntu0.16` | `1:9.9.5.dfsg-3ubuntu0.17` |
| debian | libisc95 | `1:9.9.5.dfsg-3ubuntu0.16` | `1:9.9.5.dfsg-3ubuntu0.17` |
| debian | libisccfg90 | `1:9.9.5.dfsg-3ubuntu0.16` | `1:9.9.5.dfsg-3ubuntu0.17` |
| debian | liblwres90 | `1:9.9.5.dfsg-3ubuntu0.16` | `1:9.9.5.dfsg-3ubuntu0.17` |
| debian | libtasn1-6 | `3.4-3ubuntu0.5` | `3.4-3ubuntu0.6` |
| debian | libtasn1-6-dev | `3.4-3ubuntu0.5` | `3.4-3ubuntu0.6` |
| debian | libudev-dev | `204-5ubuntu20.25` | `204-5ubuntu20.26` |
| debian | libudev1 | `204-5ubuntu20.25` | `204-5ubuntu20.26` |
| debian | udev | `204-5ubuntu20.25` | `204-5ubuntu20.26` |
| python2 | certifi | `2017.11.5` | `2018.1.18` |
| python2 | websocket-client | `0.46.0` | `0.47.0` |
| python3 | certifi | `2017.11.5` | `2018.1.18` |
| python3 | ruamel.yaml | `0.15.35` | `0.15.37` |
| python3 | websocket-client | `0.46.0` | `0.47.0` |


### 14.04.3-r15

(2018/04/03) Downloads: [img](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-r15.img.xz), [bmap](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-r15.bmap).

| property | value |
|---|---|
| base | [bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz](/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/) |
| kernel | as-is |
| applicable | bb-black, bb-green, bb-green-wireless (if applying [kernel](/embedded-linux/os/beaglebone/kernels/README.md) **4.4.39**) |

Based on [bbb-image-gen](https://github.com/yagamy4680/bbb-image-gen) (commit [82142fc029e8374b55a630fe823a6514fc7108f6](https://github.com/yagamy4680/bbb-image-gen/commit/82142fc029e8374b55a630fe823a6514fc7108f6)), build with following options:

```bash
export PATH="$PATH:/opt/yapps-env/tools/bmap-tools-3.2"
export BASE_IMAGE_URL="https://archives.t2t.io/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz"
export PRE_BUILT_PACKAGES="bluez-5.32-src,fswebcam-src,eprog-0.7.7-github,socat-1.7.3.2-src"
./gen-image ${BASE_IMAGE_URL}
```

Comparing to previous version r14, here are major changes:

- dotfiles
  - change default nodejs from `4.4.7` to `8.11.1`
  - keep nodejs `4.4.7` as optional
  - remove nodejs `6.12.3`
  - install nodejs `9.10.1` for experiments

| type | name | r14 | r15 |
|---|---|---|---|
| debian | libssl-dev | `1.0.1f-1ubuntu2.23` | `1.0.1f-1ubuntu2.24` |
| debian | libssl-doc | `1.0.1f-1ubuntu2.23` | `1.0.1f-1ubuntu2.24` |
| debian | libssl1.0.0 | `1.0.1f-1ubuntu2.23` | `1.0.1f-1ubuntu2.24` |



### 14.04.3-r16

(2018/04/03) Downloads: [img](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-r16.img.xz), [bmap](ubuntu-14.04.3-console-armhf-2016-02-11-raw-1700mb-r16.bmap).

| property | value |
|---|---|
| base | [bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz](/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/) |
| kernel | as-is |
| applicable | bb-black, bb-green, bb-green-wireless (if applying [kernel](/embedded-linux/os/beaglebone/kernels/README.md) **4.4.39**) |

Based on [bbb-image-gen](https://github.com/yagamy4680/bbb-image-gen) (commit [82142fc029e8374b55a630fe823a6514fc7108f6](https://github.com/yagamy4680/bbb-image-gen/commit/82142fc029e8374b55a630fe823a6514fc7108f6)), build with following options:

```bash
export PATH="$PATH:/opt/yapps-env/tools/bmap-tools-3.2"
export BASE_IMAGE_URL="https://archives.t2t.io/embedded-linux/os/beaglebone/mirrors/elinux.org/bb-green/bone-ubuntu-14.04.3-console-armhf-2016-02-11-2gb.img.xz"
export PRE_BUILT_PACKAGES="bluez-5.32-src,fbtftp-src,fswebcam-src,eprog-0.7.7-github,socat-1.7.3.2-src"
./gen-image ${BASE_IMAGE_URL}
```

Comparing to previous version r15, here are major changes:

- New packages: (**utilities**)
  - `curl`
  - `tcptrack`
  - `iftop`
  - `ifstat`
  - `speedometer`
  - `ethtool`
  - `ifplugd`
- New packages: (**dev-tooles**)
  - `dosfstools`
  - `initramfs-tools`
  - `u-boot-tools`
  - `rsync`
- New packages: (**daemon**)
  - `chrony` (but `ntp` is removed)
- New packages: (**libraries**)
  - `libpcap-dev`
  - `libavahi-compat-libdnssd-dev`
  - `libi2c-dev`
- New Python3 packages:
  - `sarge`
  - `fbtftp`

- dotfiles
  - change default nodejs from `4.4.7` to `8.11.1`
  - keep nodejs `4.4.7` as optional
  - remove nodejs `6.12.3`
  - install nodejs `9.10.1` for experiments

Package Differences:

| type | name | r16.csv | r15.csv |
|---|---|---|---|
| debian | avahi-utils | `0.6.31-4ubuntu1.2` | `0.6.31-4ubuntu1.1` |
| debian | dosfstools | `3.0.26-1ubuntu0.1` | `3.0.26-1` |
| debian | initramfs-tools | `0.103ubuntu4.11` | `0.103ubuntu4.2-1rcnee1~bpo1404+20151007+1` |
| debian | initramfs-tools-bin | `0.103ubuntu4.11` | `0.103ubuntu4.2-1rcnee1~bpo1404+20151007+1` |
| debian | libavahi-client3 | `0.6.31-4ubuntu1.2` | `0.6.31-4ubuntu1.1` |
| debian | libavahi-common3 | `0.6.31-4ubuntu1.2` | `0.6.31-4ubuntu1` |
| debian | libcurl3 | `7.35.0-1ubuntu2.16` | `7.35.0-1ubuntu2.15` |
| debian | libcurl4-openssl-dev | `7.35.0-1ubuntu2.16` | `7.35.0-1ubuntu2.15` |
| debian | libgcrypt11 | `1.5.3-2ubuntu4.6` | `1.5.3-2ubuntu4.5` |
| debian | libgcrypt11-dev | `1.5.3-2ubuntu4.6` | `1.5.3-2ubuntu4.5` |
| debian | libjpeg-turbo8 | `1.3.0-0ubuntu2.1` | `1.3.0-0ubuntu2` |
| debian | libjpeg-turbo8-dev | `1.3.0-0ubuntu2.1` | `1.3.0-0ubuntu2` |
| debian | libpng12-0 | `1.2.50-1ubuntu2.14.04.3` | `1.2.50-1ubuntu2.14.04.2` |
| debian | libpng12-dev | `1.2.50-1ubuntu2.14.04.3` | `1.2.50-1ubuntu2.14.04.2` |
| debian | libssl-dev | `1.0.1f-1ubuntu2.26` | `1.0.1f-1ubuntu2.24` |
| debian | libssl-doc | `1.0.1f-1ubuntu2.26` | `1.0.1f-1ubuntu2.24` |
| debian | libssl1.0.0 | `1.0.1f-1ubuntu2.26` | `1.0.1f-1ubuntu2.24` |
| debian | libudev-dev | `204-5ubuntu20.28` | `204-5ubuntu20.26` |
| debian | libudev1 | `204-5ubuntu20.28` | `204-5ubuntu20.26` |
| debian | perl | `5.18.2-2ubuntu1.6` | `5.18.2-2ubuntu1` |
| debian | perl-base | `5.18.2-2ubuntu1.6` | `5.18.2-2ubuntu1` |
| debian | perl-modules | `5.18.2-2ubuntu1.6` | `5.18.2-2ubuntu1` |
| debian | rsync | `3.1.0-2ubuntu0.4` | `3.1.0-2ubuntu0.2` |
| debian | udev | `204-5ubuntu20.28` | `204-5ubuntu20.26` |
| python2 | certifi | `2018.4.16` | `2018.1.18` |
| python2 | idna | `2.7` | `2.6` |
| python2 | netifaces | `0.10.7` | `0.10.6` |
| python2 | requests | `2.19.1` | `2.18.4` |
| python2 | urllib3 | `1.23` | `1.22` |
| python2 | websocket-client | `0.48.0` | `0.47.0` |
| python3 | PyYAML | `3.13` | `3.12` |
| python3 | certifi | `2018.4.16` | `2018.1.18` |
| python3 | idna | `2.7` | `2.6` |
| python3 | netifaces | `0.10.7` | `0.10.6` |
| python3 | psutil | `5.4.6` | `5.4.3` |
| python3 | requests | `2.19.1` | `2.18.4` |
| python3 | ruamel.yaml | `0.15.43` | `0.15.37` |
| python3 | shyaml | `0.5.2` | `0.5.0` |
| python3 | urllib3 | `1.23` | `1.22` |
| python3 | websocket-client | `0.48.0` | `0.47.0` |

Added since r16:

| type | name | version |
|---|---|---|
| debian | chrony | `1.29-1` |
| debian | curl | `7.35.0-1ubuntu2.16` |
| debian | ethtool | `1:3.13-1` |
| debian | ifplugd | `0.28-19ubuntu1` |
| debian | ifstat | `1.1-8build1` |
| debian | iftop | `1.0~pre2-5` |
| debian | install-info | `5.2.0.dfsg.1-2` |
| debian | libavahi-client-dev | `0.6.31-4ubuntu1.2` |
| debian | libavahi-common-dev | `0.6.31-4ubuntu1.2` |
| debian | libavahi-compat-libdnssd-dev | `0.6.31-4ubuntu1.2` |
| debian | libavahi-compat-libdnssd1 | `0.6.31-4ubuntu1.2` |
| debian | libnss-mdns | `0.10-6` |
| debian | libpcap-dev | `1.5.3-2` |
| debian | libpcap0.8-dev | `1.5.3-2` |
| debian | libperl5.18 | `5.18.2-2ubuntu1.6` |
| debian | libsnmp-base | `5.7.2~dfsg-8.1ubuntu3.2` |
| debian | libsnmp30 | `5.7.2~dfsg-8.1ubuntu3.2` |
| debian | libtomcrypt0 | `1.17-5` |
| debian | libtommath0 | `0.42.0-1build1` |
| debian | python-urwid | `1.1.1-1build2` |
| debian | speedometer | `2.8-1` |
| debian | tcptrack | `1.4.2-1build1` |
| debian | timelimit | `1.8-1` |
| debian | u-boot-tools | `2013.10-3` |
| python2 | urwid | `1.1.1` |
| python3 | fbtftp | `0.2` |
| python3 | sarge | `0.1.5.post0` |



## References

```text
2015-10-09 - v4.1.10-ti-r21 kernel
2015-09-11 - v4.1.6-ti-r15 kernel
2015-08-17 - v4.1.5-ti-r10 kernel
2016-02-11 - v4.1.17-ti-rt-r47 kernel
```
