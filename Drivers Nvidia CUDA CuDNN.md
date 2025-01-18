# Instalación de drivers de NVIDIA, CUDA y cuDNN en Debian/Ubuntu

## Actualizar Linux

Actualizar repositorios y paquetes de linux
```bash
sudo apt update && sudo apt upgrade -y
```

## Preinstalar dependencias

Instalar algunos paquetes necesarios
```bash
sudo apt install build-essential dkms linux-headers-$(uname -r)
```


## Instalar drivers de NVIDIA

Puedes instalar los drivers recomendados por Ubuntu (si usas Ubuntu) o especificar una versión.  Es recomendable usar la opción recomendada a menos que tengas una necesidad específica.

**Opción 1: Drivers recomendados (Ubuntu):**

```bash
ubuntu-drivers autoinstall
```

**Opción 2: Drivers específicos:**

Primero, identifica la versión del driver que necesitas. Puedes buscarla en la página web de NVIDIA.  Luego, instala la versión específica. Reemplaza `<version>` con la versión que desees.  Por ejemplo, para la versión 515:

```bash
sudo apt install nvidia-driver-<version>
```

**Configurar el driver (opcional):**
```bash
sudo nvidia-xconfig
```

## Instalar CUDA

Descargar el instalador de CUDA desde la página web de NVIDIA. Selecciona la versión para Debian/Ubuntu y la arquitectura de tu sistema.  Asegúrate de descargar el archivo `.deb` (instalador de Debian).

Una vez descargado (asumiendo que el archivo se llama `cuda.deb`):

```bash
sudo dpkg -i cuda.deb
sudo apt update
sudo apt install -f # Instalar dependencias faltantes
```

## Instalar cuDNN

1. **Descargar cuDNN:** Descarga la versión de cuDNN compatible con tu versión de CUDA desde la página web de NVIDIA. Necesitarás una cuenta de desarrollador de NVIDIA para descargarlo.  Descarga el paquete para Debian/Ubuntu.

2. **Extraer los archivos:** Extrae el archivo descargado.  Generalmente contendrá tres carpetas: `include`, `lib64`, y `bin`.

3. **Copiar los archivos:** Copia los archivos de las carpetas extraídas a las carpetas correspondientes de CUDA:

```bash
sudo cp -P cuda/include/cudnn*.h /usr/local/cuda/include/
sudo cp -P cuda/lib64/libcudnn* /usr/local/cuda/lib64/
sudo chmod a+r /usr/local/cuda/include/cudnn*.h /usr/local/cuda/lib64/libcudnn*
```

## Reiniciar el sistema

```bash
sudo reboot
```

## Verificar la instalación

```bash
nvidia-smi
```
Para verificar cuDNN, puedes compilar y ejecutar un ejemplo de CUDA que utilice cuDNN.

