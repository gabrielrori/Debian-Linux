# Instalar Python 3.8


## Actualizar lista de paquetes e instalar prerequisitos
```sh
sudo apt update
sudo apt install software-properties-common
```
## Agregar el repositorio de deadsnakes
```sh
sudo add-apt-repository ppa:deadsnakes/ppa
```
## Instalar python y herramientas de python para ambiente virtual (virtual environment)
```sh
sudo apt-get install python3.8 python3.8-dev python3.8-distutils python3.8-venv
```
Crear carpeta para archivos de Python3.8 en un ambiente virtual y acceder
```sh
mkdir /tmp/Python38
cd /tmp/Python38
```
## Instalar el ambiente virtual
```sh
sudo apt install virtualenv
python3.8 -m pip install virtualenv
```

## Acceder al ambiente virtual
```sh
virtualenv -p python3.8 venv
source venv/bin/activate
```
## Actualizar setuptools y actualizar paquetes de python
```sh
sudo python3.8 -m pip install --upgrade -U setuptools
```
```sh
sudo python3.8 -m pip install numpy scipy matplotlib ipython jupyter pandas sympy
```



## Acceder al ambiente virtual
```sh
cd /tmp/Python38
source venv/bin/activate
```
