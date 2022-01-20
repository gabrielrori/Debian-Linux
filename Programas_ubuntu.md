ANYDESK

sudo apt update
sudo apt -y upgrade

wget -qO - https://keys.anydesk.com/repos/DEB-GPG-KEY | sudo apt-key add -

echo "deb http://deb.anydesk.com/ all main" | sudo tee /etc/apt/sources.list.d/anydesk-stable.list

sudo apt update
sudo apt install anydesk

anydesk


------------------



ZOOM

sudo apt -y install wget
wget https://zoom.us/client/latest/zoom_amd64.deb
sudo apt install ./zoom_amd64.deb


sudo apt update
sudo apt install snapd
sudo snap install zoom-client


ubuntu 20.04 apr 2020
ubuntu 18.04 apr 2018

python 3.6 dec 2016
python 3.8 oct 2019


gtx 1080 2016
Tesla P100 2016

Tesla k10 2012
Tesl k40 fin 2013
