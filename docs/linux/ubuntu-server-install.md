## Remove Snaps
```
snap list
sudo snap remove --purge [app]
sudo apt remove --autoremove snapd
```
---
## Stop Snap Updating
```
sudo gedit /etc/apt/preferences.d/nosnap.pref
Package: snapd
Pin: release a=*
Pin-Priority: -10
```
---
## Update
```
sudo apt update
sudo apt upgrade

sudo apt install --only-upgrade package_names
```
## Install AwesomeWM, Xinit, Thunar, Alacritty
```
sudo add-apt-repository ppa:aslatter/ppa -y

sudo apt update

sudo apt-get install awesome awesome-extra xinit thunar alacritty pavucontrl rofi nitrogen
```
---
## Install Brave
```
sudo curl -fsSLo /usr/share/keyrings/brave-browser-archive-keyring.gpg https://brave-browser-apt-release.s3.brave.com/brave-browser-archive-keyring.gpg

echo "deb [signed-by=/usr/share/keyrings/brave-browser-archive-keyring.gpg] https://brave-browser-apt-release.s3.brave.com/ stable main"|sudo tee /etc/apt/sources.list.d/brave-browser-release.list

sudo apt update

sudo apt install brave-browser

```
---
## AutoLogin
.xinitrc
```
exec awesome
```
.bash_login
```
if [[ -z $display ]] && [[ $(tty) = /dev/tty1 ]]; then
startx
fi
```