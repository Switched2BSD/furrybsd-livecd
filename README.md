# furrybsd-livecd
LiveCD builder for FurryBSD
Dont forget to Subscribe to my Channel on Youtube:
Switched2BSD

## Install git required for furybsd-ports

```
pkg install git
```

## Customize
Add more packages to XFCE edition:
```
edit settings/packages.xfce
```

Enable more services:
```
edit settings/rc.conf.xfce
```

## Build
Generate an ISO with XFCE:
```
./build.sh
```
Generate an ISO with Gnome3:
```
./build.sh gnome
```
Generate an ISO with KDE Plasma 5:
```
./build.sh kde
```

## Burn

Burn the XFCE image to cd:
```
pkg install crdtools
cdrecord /usr/local/furybsd/iso/FuryBSD-12.1-RC2-XFCE.iso
```

Write the XFCE image to usb stick:
```
sudo dd if=/dev/usr/local/furybsd/iso/FuryBSD-12.1-RC2-XFCE.iso of=/dev/da0 bs=4m
```

## Credentials for live media
liveuser: furybsd

root: furybsd
