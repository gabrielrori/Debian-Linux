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

Escenciales python
sudo apt-get install -y build-essential \
checkinstall \
libreadline-gplv2-dev \
libncursesw5-dev \
libssl-dev \
libsqlite3-dev \
tk-dev \
libgdbm-dev \
libc6-dev \
libbz2-dev \
zlib1g-dev \
openssl \
libffi-dev \
python3-dev \
python3-setuptools \
wget libmysqlclient-dev

mkdir /tmp/Python38
cd /tmp/Python38



sudo apt-get install python3.8 python3.8-dev python3.8-distutils python3.8-venv

python3.8 -m pip install --upgrade pip

sudo apt install virtualenv
python3.8 -m pip install virtualenv



virtualenv -p python3.8 venv
source venv/bin/activate

sudo python3.8 -m pip install numpy scipy matplotlib ipython jupyter pandas sympy

sudo python3.8 -m pip install scipy ipython jupyter pandas sympy



ENTRAR
cd /tmp/Python38
source venv/bin/activate
