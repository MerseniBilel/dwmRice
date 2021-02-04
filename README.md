# dwmRice ❤️
![ArcoLinux-2021-02-04-1612467390_screenshot_1920x1080](https://user-images.githubusercontent.com/57067060/106947174-58bcfd00-672a-11eb-8e91-9ea27781f2a8.jpg)

## Requirements ⚠️
  In order to build dwm you need the Xlib header files
## Installation 💾
  1. Edit config.mk to match your local setup (default : /usr/local)
  2. Afterwards enter the following command to build and install dwm (need root)
    ..* sudo make clean install

## Running dwm 💻
Add the following line to your .xinitrc to start dwm using startx:
exec dwm
 
⚠️⚠️⚠️ In order to connect dwm to a specific display, make sure that the DISPLAY environment variable is set correctly, e.g.:
  DISPLAY=foo.bar:1 exec dwm



In order to display status info in the bar, you can do something
like this in your .xinitrc:


while xsetroot -name "`date` `uptime | sed 's/.*,//'`"
    do
        sleep 1
    done &
    exec dwm


## Configuration 📟

The configuration of dwm is done by creating a custom config.h
and (re)compiling the source code.
