# xubuntu-on-macbook-white-installation

1. Check the Mac os specifications for the 2009 model
https://everymac.com/systems/apple/macbook/specs/macbook-core-2-duo-2.13-white-13-mid-2009-nvidia-specs.html

2. Watch: Make a bootable usb disk for Mac OS<br>
https://www.youtube.com/watch?v=ughBRtJwqQI&t=81s<br>
2. 1. Install UnetBootin http://unetbootin.github.io/
2. 2. Xubuntu downloads<br
http://cdimage.ubuntu.com/xubuntu/releases/18.04/release/<br>
2. 3. Make usb disk<br>

3. Upgrade if need be<br>
https://askubuntu.com/questions/1141501/i-cant-run-sudo-apt-get-update-in-ubuntu-17-10<br>
Ubuntu 17.10 reached End Of LIFE 19th July 2018 .. you should have upgraded to 18.04 long ago.<br>
You can change fr.archive.ubuntu.com to old-releases.ubuntu.com in /etc/apt/sources.list, and then run sudo apt update and sudo apt upgrade.<br>

4. Configure wireless
https://askubuntu.com/questions/1076964/macbook-can-t-find-wifi-for-ubuntu-18-04<br>
lspci -vvnn | grep -A 9 Network -> Broadcom 4321 chipset<br>
Worked: <br>
https://askubuntu.com/questions/55868/installing-broadcom-wireless-drivers <br>

sudo apt install firmware-b43-installer <br>
sudo apt install linux-firmware <br>
sudo reboot <br>
sudo modprobe -r b43 <br>
sudo modprobe b43    <br>
sudo rfkill unblock all  <br>

Fix french canadian keyboard layout: <br>
https://askubuntu.com/questions/896551/mac-canadian-multilingual-keyboard-on-ubuntu <br>
sudo apt install --reinstall xkb-data <br>
setxkbmap -option "lv3:lalt_switch,lv3:ralt_alt,apple:badmap"<br>
