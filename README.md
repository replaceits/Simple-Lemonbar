# Simple-Lemonbar
A simple setup for lemonbar.

![Lemonbar screenshot](https://i.imgur.com/rPCohVJ.png)

## Prerequisites
[xdotool](https://github.com/jordansissel/xdotool)  
[Font Awesome](https://github.com/FortAwesome/Font-Awesome)  
[alsa-utils](https://github.com/gittup/alsa-utils)
  
## Installation  
1. Move `lemonbar.sh` to a proper directory (for EX. `/usr/local/bin`).
2. Auto start the script piped into lemon bar when your WM/DM starts. Below is an example of how I call this script in openbox (autostart file at `~/.config/openbox/autostart`)
  2. `( sleep 1s && bash /usr/local/bin/lemonbar/lemonbar.sh | lemonbar -p -F#FFFFFFFF -B#FF222222 -f "DejaVu Sans Mono"-8 -f FontAwesome-8) &`
3. You need to be sure to give `lemonbar` the arguments `-p -f "Font of your choosing"-8 -f FontAwesome-8`. The first font can be any of your choosing but the second one needs to be FontAwesome.
