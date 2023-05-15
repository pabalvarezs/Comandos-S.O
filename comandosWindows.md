# Comandos Windows #

## Comandos CMD ##

+ Usuarios Windows
~~~
netplwiz.msc
~~~
+ Directivas Grupo Local
~~~
gpedit.msc
~~~
+ Desinstalar Programas
~~~
appwiz.cpl
~~~
+ Programador de tareas
~~~
taskschd.msc
~~~
* Desfragmentador GUI
~~~
dfrgui
~~~
+ Comando Desfragmentar disco C
~~~
defrag c: /a
~~~

+ Comando Usuarios CMD
~~~
control userpasswords2
~~~
+ Directorio Fuentes
~~~
%windir%\fonts
~~~

+ DNS y Comprobar servidor
~~~
nslookup -q=MX mtca.cl
~~~
~~~
nslookup -type=any mtca.cl
~~~
+ Comprobador de Archivos Windows
~~~
sfc /scannow
~~~
---
## Examinar busca de virus ##
1.  Situarte en la carpeta antivirus
~~~
cd \Program Files\Windows Defender
~~~
2.  Ejecutar Nivel 1 - 2- 3
~~~
mpcmdrun.exe -Scan -1
~~~
~~~
mpcmdrun.exe -Scan -2
~~~
~~~
MpCmdRun -Scan -ScanType -BootSectorScan
~~~
---
## Reparar Imagen Online Windows ##
~~~
dism.exe /Online /Cleanup-Image /CheckHealth
dism.exe /Online /Cleanup-Image /ScanHealth
dism.exe /Online /Cleanup-Image /RestoreHealth 
~~~

## Información del Sistema  ##
~~~ 
msinfo32
~~~

## Comando de Estadisticas TCP/IP
+ Todas las conexiones y puertos incluidas listening
~~~
netstat -a
~~~
+ Muestra el nombre completo de dominio 
~~~
netstat -f
~~~
+ Muestra la ip y puerto del remoto
~~~
netstat -n
~~~
+ Muestra las tablas de Rutas
~~~
netstat -r
~~~
+ Muestra estadisticas
~~~
netstat -e
~~~
+ Muestra los programas que estan conectados
~~~
netstat -b
~~~
+ BUsqueda especifica 
~~~
netstat -f | findstr PALABRA
~~~
## Comando de Diskpart
+ Formatear Pendrive
~~~
diskpart

list disk

select disk [Your disk]

clean

create partition primary

format fs=ntfs

exit

~~~




