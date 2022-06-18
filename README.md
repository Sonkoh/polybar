# WorkSpace BSPWM

### Preview
<img src="https://media.discordapp.net/attachments/872254527389188157/987819035242659850/unknown.png?width=1098&height=618">

### Instalation

```sh
sudo apt update
sudo apt install build-essential git vim xcb libxcb-util0-dev libxcb-ewmh-dev libxcb-randr0-dev libxcb-icccm4-dev libxcb-keysyms1-dev libxcb-xinerama0-dev libasound2-dev libxcb-xtest0-dev libxcb-shape0-dev -y
cd ~/Descargas
git clone https://github.com/Sonkoh/polybar.git
git clone https://github.com/baskerville/bspwm.git
git clone https://github.com/baskerville/sxhkd.git
cd bspwm/
make
sudo make install
cd ../sxhkd/
make
sudo make install
sudo apt install bspwm -y
cp -r ~/Descargas/polybar/bspwm ~/.config/bspwm
cp -r ~/Descargas/polybar/sxhkd ~/.config/sxhkd
chmod +x ~/.config/bspwm/bspwmrc 
sudo apt install cmake cmake-data pkg-config python3-sphinx libcairo2-dev libxcb1-dev libxcb-util0-dev libxcb-randr0-dev libxcb-composite0-dev python3-xcbgen xcb-proto libxcb-image0-dev libxcb-ewmh-dev libxcb-icccm4-dev libxcb-xkb-dev libxcb-xrm-dev libxcb-cursor-dev libasound2-dev libpulse-dev libjsoncpp-dev libmpdclient-dev libcurl4-openssl-dev libnl-genl-3-dev -y
cd ~/Descargas/
git clone --recursive https://github.com/polybar/polybar
cd polybar/
mkdir build
cd build/
cmake ..
make -j$(nproc)
sudo make install
sudo apt update
sudo apt install meson libxext-dev libxcb1-dev libxcb-damage0-dev libxcb-xfixes0-dev libxcb-shape0-dev libxcb-render-util0-dev libxcb-render0-dev libxcb-randr0-dev libxcb-composite0-dev libxcb-image0-dev libxcb-present-dev libxcb-xinerama0-dev libpixman-1-dev libdbus-1-dev libconfig-dev libgl1-mesa-dev libpcre2-dev libevdev-dev uthash-dev libev-dev libx11-xcb-dev libxcb-glx0-dev -y
cd ~/Descargas
git clone https://github.com/ibhagwan/picom.git
cd picom/
git submodule update --init --recursive
meson --buildtype=release . build
ninja -C build
sudo ninja -C build install
sudo apt install rofi
sudo apt install firejail
cd ~/Descargas
wget https://github.com/ryanoasis/nerd-fonts/releases/download/v2.1.0/Hack.zip
sudo mv -r Hack.zip /usr/local/share/fonts/
sudo unzip /usr/local/share/fonts/Hack.zip
sudo rm /usr/local/share/fonts/Hack.zip
sudo apt install feh
cp -r ~/Descargas/polybar/Wallpapers ~/Imágenes/
```
