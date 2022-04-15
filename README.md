# Basic commands for the Linux terminal Part 2

##



*Actulizar la base de dato que almacena todas las rutas*

````bash
updatebd
````

*redirección (transladar la información)*
````bash
>
````
*adicione la salida*
````bash
>>
````
*redirecciona la salida*
````bash
<
````

#loquei
*para buscar archivos y directorios*

````bash
locate fr4nzisko.txt 
````
*para buscar programas instalados*

````bash
which nano
````

*Mostrar de manera ordenada*

````bash
tree
````

*Muestra determinadas lineas*
````bash
|
````
````bash
grep 
````
*Ignora mayusculas y minusculas*
````bash
-i
````
*Toma el inicio de una letra*
````bash
^
````
````bash
ls > lista.txt 
cat lista.txt | grep palabra
cat lista.txt | grep -i palabra 
cat lista.txt | grep ^l
cat lista.txt | grep -i ^l
````


# find (fain) para busqueda de ficheros / directorio

*Ignorar mayúsculas y minúsculas*
````bash
-iname
````
*Buscar directorios*
````bash
type d
````

*Buscar ficheros*
````bash
type f
````
*Cuando se produce un error enviar a *
````bash
2>
````

````bash
find / -name loba.txt 2>/dev/null
find /home/kali/ -name loba.txt 2>/dev/null
find /home/kali/  -iname loba.txt 2>/dev/null 
find . -type d -name clases 2>/dev/null 
find / -type f -name ".*"
find /  -name*.sh 2>/dev/null 
find / -user l0b4
````


# Busca texto que cumplan con determinado patrón
````bash
awk
````

````bash
ls -l | awk '{print $1"*" $9````'
````



# Descargas 

*Nos permite realizar descarga bajo protocolos como FTP, HTTP*
````bash
wget
````

*indicar ruta especifica de descarga*
````bash
-P
````

````bash
wget -P <url>
````

````bash
git clone <url>
````

# Instalaciones
````bash
sudo apt-get auto-remove nano
````

````bash
sudo apt-get install nano
````




# Descomprimir y comprimir 

*directorio_comprimido.zip directorio (comprimir)*
````bash
zip -r
````

*descomprimir*
````bash
unzip directorio_comprimido.zip 
````

*comprimir*
````bash
7z a nombre_directorio 
````

*descoprimir*
````bash
7z e nombre_directorio.7z 
````


# Actualizaciones

*repositorios (servicio que almacena paquetes y progrma para ser descargados)*
````bash
sudo apt-get update
````

*sistema*
````bash
sudo apt-get upgrade 
````

````bash
sudo apt-get --help
````
