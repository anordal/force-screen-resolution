force-screen-resolution
-----------------------

When your screen is stuck at 1024×768 because EDID is broken, and you just want to force it.

    > ./force-screen-resolution --help

    Usage:
    ./force-screen-resolution [options] monitor width height Hz

    Ex:
    ./force-screen-resolution HDMI-0 1920 1080 60

    Options:
    --timing=GTF|CVT|CVT-RB  Choose timing scheme. Influences the pixel clock.
        GTF = Generalized Timing Formula, see man 1 gtf
        CVT = Coordinated Video Timing, see man 1 cvt
        CVT-RB = CVT with reduced blanking (too little for CRT screens).
        default: CVT-RB

    You have 2 Monitors:
    LVDS 1600/382x900/214+0+0
    HDMI-0 1920/508x1080/286+1600+0

This script automates the [xrandr acrobatics][1] described on the arch wiki.
My contribution is public domain. Use at your own risk.

[1]: https://wiki.archlinux.org/index.php/xrandr#Adding_undetected_resolutions
