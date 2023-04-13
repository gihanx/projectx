```
snap list
sudo snap remove --purge [app]
sudo apt remove --autoremove snapd

sudo gedit /etc/apt/preferences.d/nosnap.pref
Package: snapd
Pin: release a=*
Pin-Priority: -10

sudo apt update
sudo apt upgrade


sudo apt install --only-upgrade package_names

sudo apt-get install awesome awesome-extra

sudo apt-get install xinit kitty thunar

startx


sudo add-apt-repository ppa:aslatter/ppa -y
sudo apt install alacritty

sudo apt install curl

sudo curl -fsSLo /usr/share/keyrings/brave-browser-archive-keyring.gpg https://brave-browser-apt-release.s3.brave.com/brave-browser-archive-keyring.gpg

echo "deb [signed-by=/usr/share/keyrings/brave-browser-archive-keyring.gpg] https://brave-browser-apt-release.s3.brave.com/ stable main"|sudo tee /etc/apt/sources.list.d/brave-browser-release.list

sudo apt update

sudo apt install brave-browser

```