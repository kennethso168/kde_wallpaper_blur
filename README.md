# KDE Wallpaper Blur

This script automatically detects when you change wallaper in KDE Plasma, blurs it, and sets it to your lockscreen and SDDM.

![gif](https://i.imgur.com/bLLJtNR.gif)

### Installation

You will need package `inotify-tools`. Arch linux users can install it via `pacman -S inotify-tools`. Other distros may include it by default.

```bash
$ git clone https://github.com/andreyorst/kde_wallpaper_blur.git; cd kde_wallpaper_blur
$ ./setup.sh # requires root access
```

Installation script will create image called `.bg.png` in your `$HOME` dir, and copy it to your current sddm theme folder. Then the blur script will be set to autostart, and launched for current session.
If you doing this for new user, it will ask to change your wallpaper, because there is none set in desktop config file.
No further manipulations should be needed, but if you run into trouble, open issue with step by step guide how to reproduce it.

Installation script will create backup files called \*.prewpblur in various places. Check out script output.

This software comes with no warranty.
