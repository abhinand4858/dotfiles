# i3config
Configuration file of i3-wm and i3-status configuration file

### Download Telegram Desktop and do
    mv path/to/Telegram/ ~/.Tg

### For Volume Icon
    sudo apt install volumeicon-alsa

### Wallpaper
Install feh.
Wallpaper should be here: `~/.wallpaper/wall1.png`

### Install Network Manager
    sudo apt install network-manager-gnome

### Using light for backlight control

Download the latest release from https://github.com/haikarainen/light/releases
  
      tar xf light-x.yy.tar.gz
      cd light-x.yy/
      ./configure && make
      sudo make install
      
And further add these lines to your i3 config file:

    bindsym XF86MonBrightnessUp exec light -A 5 # increase screen brightness
    bindsym XF86MonBrightnessDown exec light -U 5 # decrease screen brightness

# i3blocks configuration

Place i3blocks.conf file at this path : `~/.config/i3/i3status.conf`

# Record screen

	ffmpeg -video_size 1920x1080 -framerate 25 -f x11grab -i :0.0 output.mp4

# Make window transitions smooth

	sudo apt install xcompmgr
