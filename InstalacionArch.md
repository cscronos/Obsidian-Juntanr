# ArchLinux

**Idioma teclado**
*Este es para español, pero por defecto viene en ingles.**
```md 
loadkeys es
 ```


**Conexión Inalámbrica**
*si estas conectado por cable no es necesario hacer lo siguiente.*
```md 
iwctl 
device list 
station NOMBRE_DISPOSITIVO scan # El nombre sale del comando anterior 
station NOMBRE_DISPOSITIVO get-networks 
station NOMBRE_DISPOSITIVO connect NOMBRE_ROUTER 
exit

# comprobar si tienes internet 
ping archlinux.org 
timedatectl set-ntp true
 ```

**Particion**
*Si estas en VirtualBox*
```md 
# Enlistamos los discos. 
fdisl -l 
# Entramos a el disco donde se instalara *Arch*.
cfdisk /dev/sda 
 ```

```md 
# Enlistamos los discos. 
fdisl -l 

# Entramos a el disco donde se instalara *Arch*.
cfdisk /dev/sda 

gpt
new
521M
Type
EFI System
# seleccionas Fre

 ```