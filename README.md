# linux-bluetooth

# step 1, update bluez
sudo add-apt-repository ppa:bluetooth/bluez
sudo apt update
sudo apt install bluez

# step 2, Edit the ALSA configuration file
sudo gedit /etc/modprobe.d/alsa-base.conf
## append the following line
## options snd-hda-intel model=generic


# step 3, install blueman; 用这个这个之后配对和连接蓝牙设备变得10x容易多了
sudo apt-get install blueman

systemctl restart bluetooth
