# Instalar Python 3.7 en un ambiente virtual

## Crear carpeta para archivos de Python3.8 en un ambiente virtual y acceder
```sh
mkdir /tmp/Python37
cd /tmp/Python37
```
## Instalar python y herramientas de python para ambiente virtual (virtual environment)
```sh
sudo apt-get install python3.7 python3.7-dev python3.7-distutils python3.7-venv
```
## Actualizar pip
```sh
python3.7 -m pip install --upgrade pip
```
## Instalar el ambiente virtual
```sh
sudo apt install virtualenv
python3.7 -m pip install virtualenv
```
## Acceder al ambiente virtual
```sh
virtualenv -p python3.7 venv37
source venv37/bin/activate
```
## Actualizar setuptools y actualizar paquetes de python
```sh
sudo python3.7 -m pip install numpy scipy matplotlib ipython jupyter pandas sympy
```
```sh
sudo python3.7 -m pip install scipy ipython jupyter pandas sympy
```


## Acceder al ambiente virtual
```sh
cd /tmp/Python37
source venv37/bin/activate
```
