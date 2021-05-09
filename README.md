
# **Comandos-Linux**

## Encender Luces teclado retroilumnidado:

~~~
Teclado ON

xset led on

Teclado OFF

xset led off
~~~

## Cambiar formato hora linux - windows dualboot:

~~~
to do
~~~

## Modificar grub linux - windows dualboot:

Abrimos el archivo grub (sudo)
~~~
sudo nano /etc/default/grub
~~~
Modificamos el archivo
~~~
                     
# If you change this file, run 'update-grub' afterwards to update
# /boot/grub/grub.cfg.
# For full documentation of the options in this file, see:
#   info -f grub -n 'Simple configuration'

GRUB_DEFAULT=0
GRUB_TIMEOUT_STYLE=hidden
GRUB_TIMEOUT=10
GRUB_DISTRIBUTOR=`lsb_release -i -s 2> /dev/null || echo Debian`
GRUB_CMDLINE_LINUX_DEFAULT="quiet splash"
GRUB_CMDLINE_LINUX=""

# Uncomment to enable BadRAM filtering, modify to suit your needs
# This works with Linux (no patch required) and with any kernel that obtains
# the memory map information from GRUB (GNU Mach, kernel of FreeBSD ...)
#GRUB_BADRAM="0x01234567,0xfefefefe,0x89abcdef,0xefefefef"

# Uncomment to disable 

~~~

Luego de modificar debemos actualizar el archivo grub
~~~
sudo update-grub
~~~
