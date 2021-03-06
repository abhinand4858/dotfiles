# Ricing i3-gaps on Ubuntu 20.04
Configuration files for i3-gaps and i3-status

### Complete package list for installation

```sudo apt install libxcb1-dev libxcb-keysyms1-dev libpango1.0-dev libxcb-util0-dev libxcb-icccm4-dev libyajl-dev libstartup-notification0-dev libxcb-randr0-dev libev-dev libxcb-cursor-dev libxcb-xinerama0-dev libxcb-xkb-dev libxkbcommon-dev libxkbcommon-x11-dev autoconf xutils-dev libtool automake libxcb-xrm-dev libxcb-shape0-dev rofi volumeicon-alsa feh fonts-font-awesome compton lxappearance lxpolkit flameshot xfce4-power-manager``

```sudo apt install chromium-browser```

```sudo tar xvzf fonts.tar.xz -C /usr/share/fonts/ && cp -r .wall ~/```
  
### Download Telegram Desktop and do
    mv path/to/Telegram/ ~/.Telegram

### For Volume Icon
    sudo apt install volumeicon-alsa

### Wallpaper
Install feh.
Wallpaper should be here: `~/.wall/wall1.png`

### Rofi to search/launch apps

### Install Network Manager
    sudo apt install network-manager-gnome

### Using light for backlight control

Download the latest release from https://github.com/haikarainen/light/releases
  
      tar xf light-x.yy.tar.gz
      cd light-x.yy/
      ./autogen.sh
      ./configure && make
      sudo make install
      
And further add these lines to your i3 config file:

    bindsym XF86MonBrightnessUp exec light -A 5 # increase screen brightness
    bindsym XF86MonBrightnessDown exec light -U 5 # decrease screen brightness

# i3blocks configuration

Place i3blocks.conf file at this path : `~/.config/i3/i3status.conf`

## Record screen

	ffmpeg -video_size 1920x1080 -framerate 25 -f x11grab -i :0.0 output.mp4

## Make window transitions smooth

	sudo apt install xcompmgr

### Install lxappearance(change themes and icons) lxpolkit (user auths) flameshot (screenshot utility) 
	sudo apt install lxappearance lxpolkit flameshot

## Themes and icons

 - https://github.com/EliverLara/Sweet-folders #individual folders of icons
 - https://github.com/EliverLara/Ant
 - https://github.com/EliverLara/Sweet

	git submodule update --init --recursive
	git pull --recurse-submodule
	mkdir ~/.local/share/icons
	sudo cp -r themes/Ant/ /usr/share/themes/
	cp themes/Sweet-folders/* ~/.local/share/icons/

And further apply theme and icon using lxappearance. My take -Ant/sweet-teal-filled/Dejavu-Sans-Mono-Book
	
### colour scheme for terminal

https://github.com/Mayccoll/Gogh

