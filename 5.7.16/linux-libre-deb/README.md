# linux-libre-deb package for Void Linux

This package provides Linux-libre, the Linux kernel without binary blobs. From project [webpage](https://www.fsfla.org/ikiwiki/selibre/linux-libre/):

> GNU Linux-libre is a project to maintain and publish 100% Free distributions of Linux, suitable for use in Free System Distributions, removing software that is included without source code, with obfuscated or obscured source code, under non-Free Software licenses, that do not permit you to change the software so that it does what you wish, and that induces or requires you to install additional pieces of non-Free Software.

**WARNING:** It does not have some drivers for hardware which need binary blobs to run, so you may face difficulties on some setups. This build is very experimental. Do not remove your other Linux kernels yet and do not rely on it's stability. Do not install and do not use on your production system. I am not responsible for any damage to your system.

This package merely takes the .deb release version from the authors, extracts and installs the files similar to DEB. It does not build from source. So this is not a proper package per se.

The template file is prepared for use with [xbps-src](https://wiki.voidlinux.org/Xbps-src) in Void Linux.


## Installation
```
sudo xbps-install xtools
git clone https://github.com/void-linux/void-packages
cd void-packages
./xbps-src binary-bootstrap
# Do the above once if not done already.
# Copy this `linux-libre-deb` folder under `srcpkgs` folder, then...
./xbps-src pkg linux-libre-deb
xi linux-libre-deb
```


**Help from:**

- [Linux-libre homepage](https://www.fsfla.org/ikiwiki/selibre/linux-libre/)
