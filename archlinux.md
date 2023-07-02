## some tips
### add consolas font
```
git clone https://aur.archlinux.org/consolas-font.git
sudo pacman -S xorg-font-util
makepkg
sudo pacman -U consolas-font-1.2-2-any.pkg.tar.zst
```
### caps lock as ctrl
add this line to `~/.Xmodmap`
```
clear lock
clear control
keycode 66 = Control_L
add control = Control_L Control_R
```                                                                                                                                           

### add ru keyboard layout(hack method)
```
localectl set-keymap us ru
touch ~/.xprofile
echo "setxkbmap us,ru -option 'grp:alt_space_toggle'" >> ~/.xprofile
```
restart x session
