## Pine64 PineNote Debian

This github organization holds various repositories used to generate Debian images for the Pine64 PineNote (https://wiki.pine64.org/wiki/PineNote).
As with most of the software for Pine64 devices, this is a purely community-based effort. Please also note that, as of Jan. 2024, the PineNote was only released as a limited early-developer device.

### Notable components

* The main Debian image is generated and released using this repository: https://github.com/PNDeb/pinenote-debian-image (make sure to check with the Pine64 PineNote chat which release to flash - sometimes one of the CI-builds is more appropriate).
* The kernel used for this Debian image is maintained here: https://github.com/m-weigand/linux
* A GNOME extension is maintained for easy access to some PN-specific functionality: https://github.com/PNDeb/pinenote-gnome-extension
* TODO: https://github.com/PNDeb/pinenote-gnome-shell
* TODO: https://github.com/PNDeb/pinenote-gnome-mutter
* A rust-based dbus daemon is used to control some of the PN-related functionality (also used by the GNOME extension): https://github.com/PNDeb/pinenote_dbus_service
* Efforts are made to move PN-specific configuration into Debian packages: https://github.com/PNDeb/pinenote-tweaks
* Some work was done to implement dithering/Y4 conversion using the rk356x-included RGA hardware. Test code can be found here: https://github.com/PNDeb/rga-v4l2-demo
  
A few packages were backported/packaged to Debian bookworm:

* libinput: https://github.com/PNDeb/libinput_backport
* uMTP-reponder (used for USB gadget MTP mode) https://github.com/PNDeb/uMTP-Responder-debian
