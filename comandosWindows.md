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
## Reinstalar Archivos Imagen Online Windows ##
~~~
dism.exe /Online /Cleanup-Image /RestoreHealth 
~~~

