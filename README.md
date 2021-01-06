# power-menu-for-archlinux

* [power-menu to polybar] ( hefflogout from HefftorLinux )

## Preview

## powermenu-on
![powermenu-on](/preview/powermenu-on.png)

* Distro: [ArchLabs](https://archlabslinux.com/)
* Window manager: [Bspwm](https://github.com/Airblader/i3)
* Bar: [Polybar](https://github.com/polybar/polybar)
* Compositor [picom (kawase-blur)](https://github.com/ibhagwan/picom)


### Other prerequisites
* [betterlockscreen] (https://github.com/pavanjadhaw/betterlockscreen)
* [bc] (sudo pacman -S bc)



1- add this module to your polybar config:

[module/powermenu]
type = custom/script

exec = echo ""

;;exec = echo " "

interval = 1

tail = true

format-foreground = ${colors.foreground}

format-background = ${colors.background}

format-prefix-foreground = #738adb

format-underline = ${colors.foreground-alt}

click-left = hefflogout &

label = %output%


2- copy all files to the correct address...


3- install the requirements for the lockscreen option.


4- Updating image cache(required)
betterlockscreen -u /usr/share/backgrounds/hefftorlinux_4k/woman-music-fantacy.jpg  "or change the wall to whatever you want"

refresh polybar & enjoy your new option.
