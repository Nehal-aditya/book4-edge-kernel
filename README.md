## About

Linux & DTS to allow booting on the X1P42100 Samsung Galaxy Book4 Edge 15.6, derived from [zensanp/linux-book4-edge](https://github.com/zensanp/linux-book4-edge), as these devices seem to share some similarities. Essentials working, but some things remain untested.

## Status
Supported features:
- [x] Keyboard - needs udev [quirk](https://bugs.launchpad.net/ubuntu-concept/+bug/2084591/comments/87)
   - [x] Keyboard backlight - via OpenBSD's [samsabi](https://cvsweb.openbsd.org/log/src/sys/dev/i2c/samsabi.c,v?sort=File)
- [x] Touchpad
- [x] USB type-c
  - [ ] USB hotplug
  - [ ] DP Altmode
- [x] UFS storage
- [ ] HDMI port on the right side (not tested.)
- [x] Built-in display
- [x] GPU - needs firmware + updated Mesa
- [x] Wifi - needs firmware.
- [x] BT - needs firmware + MAC address must be set [manually](https://github.com/zensanp/linux-book4-edge/issues/5) for device.
- [x] ADSP and CDSP - need firmware
  - [x] Battery indicator - needs separate [driver](https://github.com/zensanp/linux-book4-edge/issues/4)
- [ ] Audio - untested (no HW protection. Proceed at own risk.)
  - [ ] Mic
- [x] Sleep - Does it work? [Yes]. Does it save power? [Not really].
- [x] Webcam - Needs libcamera patch
