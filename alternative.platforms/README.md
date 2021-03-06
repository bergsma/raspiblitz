# ⚡️ Alternative platforms for the RaspiBlitz ⚡️

Minimum requirements:
* ARM V7 or V8 processor architecture (32 or 64 bit)
* 1 GB RAM
* \> 300 GB HDD

Desirable:
* \> 2GB DDR3 RAM
* USB 3.0 or SATA connector
* SSD
* Compact case with efficient cooling (heatsink / fan)
* HDMI / GPIO screen


Specifications of the tested hardware: [hw_comparison.md](hw_comparison.md)

All testers are welcome. Open an issue for your specific board to collaborate and share your experience.

---
## Armbian
Many SBC-s are supported:
https://www.armbian.com/download/

Tested on:
* Odroid XU4 with the Armbian Stretch image from https://www.armbian.com/odroid-xu4/


Burn the image to the SDCard with [Etcher](https://www.balena.io/etcher/).

Assemble and boot.

`ssh root@192.168.1.122`

password: 1234

Follow the instructions in the terminal.

Continue with building the SDcard: https://github.com/rootzoll/raspiblitz#build-the-sd-card-image

---

## Ubuntu

A common distro to be supplied by the manufacturer for various boards.

Tested on:
* Odroid XU4 with ubuntu-18.04.1-4.14-minimal image from https://de.eu.odroid.in/ubuntu_18.04lts/XU3_XU4_MC1_HC1_HC2

Burn the image to the SDCard with [Etcher](https://www.balena.io/etcher/).

Assemble and boot.

`ssh root@192.168.1.122`

password: odroid

`apt-get update`

`apt-get upgrade`

if there is an error:
>E: Could not get lock /var/lib/dpkg/lock-frontend - open (11: Resource temporarily unavailable)

>E: Unable to acquire the dpkg frontend lock (/var/lib/dpkg/lock-frontend), is another process using it?

run:
`reboot` and update as above

Continue with building the SDcard: https://github.com/rootzoll/raspiblitz#build-the-sd-card-image

---

## DietPi

Many SBC-s are supported:
https://dietpi.com/#download

Tested on:

* Odroid HC1
* Odroid HC2 (the same board with a 3.5" 12V HDD)
* Odroid XU4 (with HDMI screen)
* Raspberry Pi 3 B+ (with the default GPIO or HDMI display)


The HDMI screen tested: https://www.aliexpress.com/item/3-5-inch-LCD-HDMI-USB-Touch-Screen-Real-HD-1920x1080-LCD-Display-Py-for-Raspberri/32818537950.html

Detailed instructions for the RaspiBlitz-on-DietPi: [/dietpi/README.md](/dietpi/README.md)

---
Extras for advanced users and powerful hardware:
https://github.com/openoms/bitcoin-tutorials/