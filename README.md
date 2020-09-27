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
https://askubuntu.com/questions/1076964/macbook-can-t-find-wifi-for-ubuntu-18-04
lspci -vvnn | grep -A 9 Network -> Broadcom 4321 chipset
