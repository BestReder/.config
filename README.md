# 我的配置

这个配置文件夹包括`i3`和`alacritty`配置，但是现在我使用的是`dwm`和`alacritty`

# archlinuxcn(163源)

在`/etc/pacman.conf`文件末尾添加以下内容：

```
[archlinuxcn]
SigLevel = Optional TrustedOnly
Server = http://mirrors.163.com/archlinux-cn/$arch
```

之后安装 archlinuxcn-keyring 包导入 GPG key

# blackarch(中科大源)

在 `/etc/pacman.conf` 文件末尾添加两行：

```
[blackarch]
SigLevel = Optional TrustAll
Server = https://mirrors.tuna.tsinghua.edu.cn/blackarch/$repo/os/$arch
```

然后请安装 `blackarch-keyring` 包以导入 GPG key。

## Ranger

use `pip install ueberzug` and `ranger-git`

## 安装输入法

Install: `fcitx` `fcitx-im` `fcitx-googlepinyin` `fcitx-configtool`

And in `/etc/X11/xinit/xinitrc`:

```
export GTK_IM_MODULE=fcitx
export QT_IM_MODULE=fcitx
export XMODIFIERS="@im=fcitx"
```

#### Fcitx用户需要将第一个输入法设置为键盘-布局

## fonts

#### My Font

I use the `Source Code Pro` font and `nerd-fonts-source-code-pro`.

#### About Noto

Just install `noto-fonts` (not `-all`). It's already bloated. Check `/usr/share/fonts/noto`

#### Emoji

```
yay -S ttf-linux-libertine ttf-inconsolata ttf-joypixels ttf-twemoji-color noto-fonts-emoji ttf-liberation ttf-droid
```

#### Chinese

```
yay -S wqy-bitmapfont wqy-microhei wqy-microhei-lite wqy-zenhei adobe-source-han-mono-cn-fonts adobe-source-han-sans-cn-fonts adobe-source-han-serif-cn-fonts
```

## Arch Packages I Installed:

```
i3lock
i3lock-fancy-git
acpi
acpitool
adapta-gtk-theme
adobe-source-code-pro-fonts
adobe-source-han-mono-cn-fonts
adobe-source-han-mono-tw-fonts
adobe-source-han-sans-cn-fonts
adobe-source-han-sans-tw-fonts
adobe-source-serif-pro-fonts
alacritty
alsa-utils
arc-icon-theme
autoconf
automake
base
bash-language-server
bc
binutils
bison
chromium
ctags
dbus-glib
dhcp
dhcpcd
dunst
efibootmgr
ethtool
fakeroot
fcitx
fcitx-configtool
fcitx-gtk2
fcitx-gtk3
fcitx-libpinyin
fcitx-qt5
feh
flex
fuse2
fzf
gcc
git
gnome-screenshot
google-chrome
groff
grub
htop
intel-media-driver
kdenlive
kjv-apocrypha
lazygit
libreoffice-fresh
libtool
linux
linux-firmware
llpp
lxappearance
m4
make
mono
mutt-wizard-git
neofetch
neomutt
neovim
nerd-fonts-source-code-pro
network-manager-applet
npm
os-prober
pam-gnupg-git
patch
picom-git
pkgconf
python
python-pip
python2
python2-pip
ranger-git
screenkey
simplescreenrecorder
smartmontools
sudo
terminus-font
texinfo
thunar
tlp
trayer
ttf-font-awesome
ttf-i.bming
ttf-inconsolata
ttf-joypixels
ttf-linux-libertine
ttf-symbola
ttf-twemoji-color
unzip
vlc
w3m
wget
which
wireless_tools
wpa_supplicant
wqy-bitmapfont
wqy-microhei
wqy-microhei-lite
wqy-zenhei
xclip
xdialog
xf86-video-intel
xfce4-power-manager
xfce4-volumed-pulse
xorg-docs
xorg-fonts-100dpi
xorg-fonts-75dpi
xorg-iceauth
xorg-luit
xorg-server
xorg-server-common
xorg-server-devel
xorg-server-xdmx
xorg-server-xephyr
xorg-server-xnest
xorg-server-xvfb
xorg-server-xwayland
xorg-sessreg
xorg-setxkbmap
xorg-smproxy
xorg-x11perf
xorg-xauth
xorg-xbacklight
xorg-xcmsdb
xorg-xcursorgen
xorg-xdpyinfo
xorg-xdriinfo
xorg-xev
xorg-xgamma
xorg-xhost
xorg-xinit
xorg-xinput
xorg-xkbcomp
xorg-xkbevd
xorg-xkbutils
xorg-xkill
xorg-xlsatoms
xorg-xlsclients
xorg-xmodmap
xorg-xpr
xorg-xprop
xorg-xrandr
xorg-xrdb
xorg-xrefresh
xorg-xset
xorg-xsetroot
xorg-xvinfo
xorg-xwd
xorg-xwininfo
xorg-xwud
yay
zip
zsh
```

