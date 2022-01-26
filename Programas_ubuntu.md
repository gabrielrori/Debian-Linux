# Programas para Ubuntu

## Anydesk
### Refrescar lista de repositorios e instalar actualizaciones
```sh
sudo apt update
sudo apt -y upgrade
```
### Agregar repositorio de Anydesk y clave
```sh
wget -qO - https://keys.anydesk.com/repos/DEB-GPG-KEY | sudo apt-key add -
```
### Añadir PPA al sistema
```sh
echo "deb http://deb.anydesk.com/ all main" | sudo tee /etc/apt/sources.list.d/anydesk-stable.list
```
### Actualizar lista de repositorios
```sh
sudo apt update
```
### Instalar Anydesk
```sh
sudo apt install anydesk
```
-------------------------------------------------------------------------------------------


## Zoom Client
### Instalar con Wget
#### Instalar Wget
```sh
sudo apt -y install wget
```
#### Descargar zoom con wget
```sh
wget https://zoom.us/client/latest/zoom_amd64.deb
```
#### Instalar Zoom Client
```sh
sudo apt install ./zoom_amd64.deb
```
### Instalar con Snapd
#### Instalar Snapd
#### Actualizar lista de repositorios
```sh
sudo apt update
```
#### Instalar Snapd
```sh
sudo apt install snapd
```
#### Descargar e instalar Zoom Client con Snapd
```sh
sudo snap install zoom-client
```
