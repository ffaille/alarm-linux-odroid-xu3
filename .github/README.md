This repository hosts a fork of the official [core/linux-odroid-xu3 PKGBUILD](https://github.com/archlinuxarm/PKGBUILDs/tree/master/core/linux-odroid-xu3). It allows you to build the linux-odroid-xu3 package which provides the kernel for the ODROID XU3/XU4/HC1/HC2/MC1 (v6.1.67 from Hardkernel).

The goal of this project is to offer an up-to-date version while remaining as close as possible to the productions of the official maintainer. Maybe this code can be pushed into the official repository later...

Tested with XU4 only (don't have XU3/HC1/HC2/MC1). Seems to work fine. Feedback is welcome.

## Usage
* sudo pacman -S base-devel git
* git clone https://github.com/ffaille/alarm-linux-odroid-xu3.git
* cd alarm-linux-odroid-xu3
* makepkg --syncdeps --noconfirm --log
* sudo pacman -U ./linux-odroid-xu3-6.1.67-1-armv7h.pkg.tar.xz
* sudo reboot