# Actualizar Ubuntu

```sh
sudo apt update
sudo apt upgrade
```

## Confirmar firewall deshabilitado
```sh
sudo ufw status
```

## Deshabilitar servidor de visualización Wayland

Editar archivo de configuración

```sh
sudo nano /etc/gdm3/custom.conf
```
Cambiar:
```sh
WaylandEnable=true
```
Por:
```sh
WaylandEnable=false
```
Reiniciar GDM3:
```sh
sudo systemctl restart gdm3
```

# Actualizar Python 3
Actualizar pip3 y setuṕtools

```sh
sudo apt install python3-pip python3-setuptools python3-numpy python3-matplotlib python3-scipy python3-pandas python3-sympy python3-dev jupyter-notebook
```
