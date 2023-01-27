# Hyprland config files from Titus

![Screenshot](https://github.com/ChrisTitusTech/hyprland-titus/raw/main/hyprland-titus.png)

## Install
### Yay

Run as user NOT ROOT!
```
git clone https://aur.archlinux.org/yay-bin
cd yay-bin
makepkg -si
```

### Packages
```
yay -S hyperland-bin sddm-git kitty waybar-hyprland vim tldr nano micro brave-bin dolphin vscode json-c curl cmake python-pip libappindicator-gtk3 github-desktop-bin
```

## Configuration sddm
```
Session=Hyprland.desktop
User=Jens
Numlock=true
```

## Install nerd font
```
mkdir -p $HOME/Downloads```/nerdfonts/
cd $HOME/Downloads/"
wget https://githubcom/ranoasis/nerd-fonts/releases/download/v2.3.1/CascadiaCode.zip
unzip '*.zip' -d $HOME/Downloads/nerdfonts/
rm -rf *.zip
sudo cp -R $HOME/Downloads/nerdfonts/ /usr/share/fonts/
```
## waybar weather
### Install python module
```
pip install requests
```
## Install nvidia drivers
```
yay -S nvidia
```
## Install kde
```
yay -S plsama kde-applications plasma-wayland-session
```
- Global Theme used: [Utterly Sweet](https://store.kde.org/p/1906500)
- SDDM   Theme used: [Sweet](https://github.com/EliverLara/Sweet/tree/nova/kde/sddm)
## Sources used making these

- Official Hyprland Github <https://github.com/hyprwm/Hyprland>
- Linux Mobiles Hyprland dot files <https://github.com/linuxmobile/hyprland-dots>
