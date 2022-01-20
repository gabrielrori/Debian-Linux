# Instalar Python 3.8


Run the following commands as root or user with sudo access to update the packages list and install the prerequisites:
```sh
sudo apt update
sudo apt install software-properties-common
```
Add the deadsnakes PPA to your system’s sources list:
```sh
sudo add-apt-repository ppa:deadsnakes/ppa

sudo apt-get install python3.8 python3.8-dev python3.8-distutils python3.8-venv

sudo python3.8 -m pip install --upgrade -U setuptools
```
```sh
sudo python3.8 -m pip install numpy 
sudo python3.8 -m pip install scipy 
sudo python3.8 -m pip install matplotlib 
sudo python3.8 -m pip install ipython 
sudo python3.8 -m pip install jupyter 
sudo python3.8 -m pip install pandas 
sudo python3.8 -m pip install sympy
```
