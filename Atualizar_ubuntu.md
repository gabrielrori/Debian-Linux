#Actualizar Ubuntu

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
```sh
Por:
```sh
WaylandEnable=false
```
