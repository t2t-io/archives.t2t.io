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


## References

```text
2015-10-09 - v4.1.10-ti-r21 kernel
2015-09-11 - v4.1.6-ti-r15 kernel
2015-08-17 - v4.1.5-ti-r10 kernel
2016-02-11 - v4.1.17-ti-rt-r47 kernel
```
