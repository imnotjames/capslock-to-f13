# CAPSLOCK TO F15 ![F15](http://i.imgur.com/SaN2LIF.png)
## BECAUSE CAPSLOCK IS NOT SO COOL

THIS IS A QUICK UDEV HWDB RULE TO REMAP CAPSLOCK TO F15,
BECAUSE HITTING CAPSLOCK ACCIDENTALLY CAN BE QUITE AWFUL.
IT GIVES YOU A BRAND NEW KEY TO MAP TO, INSTEAD OF YET
ANOTHER CONTROL KEY.

### INSTALLATION

IF YOU ARE USING ARCH LINUX JUST USE THE `PKGBUILD` FILE WITH
`makepkg` AND INSTALL THE RESULTING PACKAGE.

```
makepkg
pacman -U capslock-to-f15-0.0.1-1-any.pkg.tar.xz
systemctl restart udev
```

IF YOU ARE NOT USING ARCH LINUX OR WANT TO INSTALL THIS MANUALLY,
IT'S PRETTY EASY.

* COPY THE HWDB FILE TO `/etc/udev/hwdb.d/90-capslock-to-f15.hwdb`
* RUN THE UDEV HWDB UPDATE COMMAND `udevadm hwdb --update`
* RESTART UDEV
