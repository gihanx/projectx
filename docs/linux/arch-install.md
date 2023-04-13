```
timedatectl set-ntp true 

cfdisk
500MB EFI
8G SWAP
REST LINUX FILE SYSTEM

mkfs.ext4 /dev/root_partition
mkswap /dev/swap_partition
swapon /dev/swap_partition
mkfs.fat -F 32 /dev/efi_system_partition

mount /dev/root_partition /mnt

mkdir /mnt/boot
mount /dev/sda1 /mnt/boot

edit pacman.conf > multilb,extra,fastdownload

pacstrap /mnt base base-devel linux linux-firmware neovim bash-completion intel-ucode

genfstab -U /mnt >> /mnt/etc/fstab

check /mnt/etc/fstab

arch-chroot /mnt

ln -sf /usr/share/zoneinfo/Asia/Colombo /etc/localtime

hwclock --systohc

uncomment en_US.UTF-8
locale-gen

echo archlinux > /etc/hostname
edit /etc/hosts
127.0.0.1	localhost
::1		localhost
127.0.0.1	archlinux.localdomain	archlinux


pacman -S networkmanager
systemctl enable NetworkManager

passwd

bootctl install

nvim /boot/loader/loader.conf
default  arch
timeout  5
editor   no

nvim /boot/loader/entries/arch.conf
title ARCHLINUX
linux /vmlinuz-linux
initrd /initramfs-linux.img
initrd  /intel-ucode.img
options root=/dev/sda3 rw

cp /boot/loader/entries/arch.conf /boot/loader/entries/arch-fallback.conf
nvim /boot/loader/entries/arch-fallback.conf
title Arch Linux Fallback
linux /vmlinuz-linux
initrd /initramfs-linux-fallback.img
options root=/dev/sda3 rw

cp /boot/loader/entries/arch.conf /boot/loader/entries/arch-terminal.conf
title Arch Linux Terminal
linux /vmlinuz-linux
initrd /initramfs-linux.img
options root=/dev/sda3 rw systemd.unit=multi-user.target

systemctl enable systemd-boot-update.service

bootctl list

umount /mnt
exit
reboot

edit /etc/pacman.conf set extra/fastdownload

useradd -m -g users -G audio,video,network,wheel,storage,rfkill -s /bin/bash gihan
passwd gihan
EDITOR=nvim visudo

sudo pacman -Syu

sudo pacman -S --needed base-devel
git clone https://aur.archlinux.org/paru.git
cd paru
makepkg -si

paru -S hyprland-bin
```