# Magisk built-in BusyBox

### Description
Systemless Magisk module to install **BusyBox** binary with its applets (**UNIX/Linux command-line utilities**).
BusyBox and applets are installed by and symlinked to the Magisk built-in busybox binary.
For more info, see:
https://github.com/topjohnwu/ndk-busybox

**Tip**: For even more interesting applets, install also the **ToyBox-Ext** module:
https://github.com/Magisk-Modules-Alt-Repo/ToyBox-Ext

##### TEST

**Install** the module and **reboot**. Use **Terminal Emulator** - **BusyBox applets** are for Terminal and **shell scripts**.

Make sure that `/system/bin` and `/system/xbin` (the latter might not available on some devices) are in the `PATH`.
Check e.g. with (all commands are **case sensitive**):
```
su
echo $PATH
```
Check if `busybox` was properly installed and is it installed to `/system/xbin` or `/system/bin`:
```
busybox --help
which busybox
```
If the responded busybox path was `/system/xbin` then check:
```
ls -l /system/xbin | grep busybox
```
whereas if the busybox path was `/system/bin` then use:
```
ls -l /system/bin | grep busybox
```
The command will show all the busybox applets as installed (symlinked to the busybox binary).
Usually, `whois` will be one of them, hence you can try:
```
whois --help
busybox whois --help
```

### Coffee
If this module is useful for you, please support development by donating a [coffee](https://zgfg.github.io/PayPal.html)

#### Source 

[My Repo:](https://github.com/zgfg/BuiltIn-BusyBox)

![GitHub release (latest by date)](https://img.shields.io/github/v/release/zgfg/BuiltIn-BusyBox?label=Release&style=plastic) ![GitHub Release Date](https://img.shields.io/github/release-date/zgfg/BuiltIn-BusyBox?label=Release%20Date&style=plastic) 
![GitHub Releases](https://img.shields.io/github/downloads/zgfg/BuiltIn-BusyBox/latest/total?label=Downloads%20%28Latest%20Release%29&style=plastic)
![GitHub All Releases](https://img.shields.io/github/downloads/zgfg/BuiltIn-BusyBox/total?label=Total%20Downloads%20%28All%20Releases%29&style=plastic)

[Alt-Repo:](https://github.com/Magisk-Modules-Alt-Repo/BuiltIn-BusyBox)

![GitHub release (latest by date)](https://img.shields.io/github/v/release/Magisk-Modules-Alt-Repo/BuiltIn-BusyBox?label=Release&style=plastic) ![GitHub Release Date](https://img.shields.io/github/release-date/Magisk-Modules-Alt-Repo/BuiltIn-BusyBox?label=Release%20Date&style=plastic) 
![GitHub Releases](https://img.shields.io/github/downloads/Magisk-Modules-Alt-Repo/BuiltIn-BusyBox/latest/total?label=Downloads%20%28Latest%20Release%29&style=plastic)
![GitHub All Releases](https://img.shields.io/github/downloads/Magisk-Modules-Alt-Repo/BuiltIn-BusyBox/total?label=Total%20Downloads%20%28All%20Releases%29&style=plastic)

#### Copyright (c) zgfg @ xda, 2022-

