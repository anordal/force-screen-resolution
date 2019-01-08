force-screen-resolution
-----------------------

When your screen is stuck at 1024×768 because EDID is broken, and you just want to force it.

    > ./force-screen-resolution --help

    Usage:
    ./force-screen-resolution monitor width height Hz

    Ex:
    ./force-screen-resolution HDMI-0 1920 1080 59.94

    2 Monitors:
    LVDS 1600/382x900/214+0+0
    HDMI-0 1920/508x1080/286+1600+0

This script automates the [xrandr acrobatics][1] described on the arch wiki.
My contribution is public domain. Use at your own risk.

[1]: https://wiki.archlinux.org/index.php/xrandr#Adding_undetected_resolutions
