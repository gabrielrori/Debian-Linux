mkdir /tmp/Python37
cd /tmp/Python37

sudo apt-get install python3.7 python3.7-dev python3.7-distutils python3.7-venv

python3.7 -m pip install --upgrade pip

sudo apt install virtualenv
python3.7 -m pip install virtualenv



virtualenv -p python3.7 venv37
source venv37/bin/activate

sudo python3.7 -m pip install numpy scipy matplotlib ipython jupyter pandas sympy

sudo python3.7 -m pip install scipy ipython jupyter pandas sympy



ENTRAR
cd /tmp/Python37
source venv37/bin/activate



pip list
