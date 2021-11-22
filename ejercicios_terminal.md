# EJERCICIOS TERMINAL LINUX

## 1- ACTUALIZACIÓN OS UBUNTU/MINT.

### 1.1- SINCRONIZAR BASE DE DATOS LOCAL Y REPOSITORIO

sudo apt-get update

### 1.2- VISUALIZAR LOS PROGRAMAS A ACTUALIZAR

sudo apt list --upgradable

### 1.3- ACTUALIZAR NUESTRO SISTEMA OPERATIVO

sudo apt-get upgrade


## 2.- DETERMINAR CON UN COMANDO NUESTRA POSICIÓN EN EL ÁRBOL DE USUARIO

pwd


## 3- VISUALIZAR CON UN COMANDO EL ÁRBOL DEL USUARIO DESDE /home/nuestroUsuario/

tree /home/k
[]: # (Mi usuario es k)


## 4- CREAR EN /home/nuestroUsuario/ UN FOLDER LLAMADO "ejercicios".

mkdir /home/k/ejercicios


## 5- VERIFICAR SU CREACIÓN EN EL LUGAR CORRECTO, Y SU POSICIÓN EN EL ÁRBOL.

ls /home/k
tree


## 6- MOVERNOS A LA CARPETA "ejercicios" y VERIFICAR CON EL COMANDO QUE ESTAMOS AHÍ.

cd /home/k/ejercicios
pwd


## 7- CREAR ARCHIVO DE TEXTO EN FOLDER "ejercicios", ESCRIBIR TEXTO Y SALVARLO CON EL NOMBRE parte_1

nano parte_1
[]: # (Se escribe texto y se salva el fichero)


## 8- RETROCEDER A /home/k USANDO EL COMANDO DE RETROCESO O DE PATH ABSOLUTO. VERIFICAR POSICIÓN.

cd ..
[]: # (o bien, cd /home/k)
pwd


## 9- CON EL COMANDO PARÁMETROS ADECUADOS GENERAR UN LISTADO (DE ARCHIVOS).

ls -l


## 10- AGREGAR NUEVO PARÁMETRO AL COMANDO ANTERIOR PARA MOSTRAR ARCHIVOS OCULTOS.

ls -lh


## 11- DESDE /home/k/ CREAR OTRO ARCHIVO DE TEXTO LLAMADO parte_2.

nano parte_2
[]: # (Se escribe texto que se desee y se salva el fichero)


## 12- DESDE LA RAÍZ DE USUARIO CREAR UN FOLDER LLAMADO "trabajos".

mkdir trabajos


## 13- DESDE LA RAIZ DE USUARIO CREAR (en "trabajos"?) ARCHIVO DE TEXTO LLAMADO "parte_3", QUE SALVAMOS Y VERIFICAMOS ESTÉ EN EL LUGAR CORRECTO.

nano ./trabajos/parte_3
[]: # (Escribimos el texto que fuere)
ls parte_3


## 14- DESDE LA RAIZ DE USUARIO ABRIR LOS TRES ARCHIVOS, AGREAGAR NUESTRO NOMBRE AL FINAL DE CADA UNO, SALVAR Y SLIR DEL EDITOR.

cd ..
echo karel >> /ejercicios/parte_1
echo karel >> parte_2
echo karel >> ./trabajos/parte_3


## 15- NOS DIRIGIMOS AL FOLDER EN EL QUE ESTÁ "parte_3". VERIFICAR UBICACIÓN.

cd trabajos
pwd


## 16- CON EL COMANDO ADECUADO COPIAR "parte_3" EN FOLDER EN QUE ESTÁN LOS OTROS ARCHIVOS. VERIFICAR CON "tree".

mv parte_3 /home/k/ejercicios
cd ..
mv parte_2 ./ejercicios
[]: # (lo anterior faltaba, tal vez por malinterpretación mía del enunciado)

## 17- DESDE POSICIÓN ACTUAL EN ÁRBOL NOS MOVEMOS AL FOLDER EN QUE ESTÁN LOS TRES ARCHIVOS. VERIFICAMOS.

cd ejercicios
pwd


## 18- USAR COMANDO ADECUADO PARA LISTAR ARCHIVOS DEL FOLDER ACTUAL.

ls


## 19- CON EL COMANDO ADECUADO PARA LEER LOS TRES ARCHIVOS SIMULTANEAMENTE VISUALIZAMOS SUS TEXTOS EN LÍNEAS SEPARADAS.

cat parte_1 parte_2 parte_3


## 20- CONCATENAR LOS TRES ARCHIVOS Y LLAMAR AL NUEVO ARCHIVO "textoTotal".

cat parte_1 parte_2 parte_3 > textoTotal


## 21- LISTAR LOS ARCHIOVOS DEL FOLDER Y VERIFICAR SI ESTÁ "textoTotal".

ls


## 22- ABRIR "textoTotal" con el editor y escribir "trabajo finalizado". SALVAR y SALIR.

nano textoTotal
[]: # (escribir texto...)


## 23- BORRAMOS EL FOLDER "trabajos".

cd ..
rm trabajos/ -fr


## 24- NOS MOVEMOS A "/home/k/

cd /home/k


## 25- CREAR DESDE LA RAÍZ DEL USUARIO UN FOLDER LLAMADO "final".

mkdir final


## 26- COPIAR ARCHIVO "textoTotal" DESDE SU UBICACIÓN AL FOLDER "final" USANDO PATH ABSOLUTO.

cp /home/k/ejercicios/textoTotal /home/k/final/


## 27- BORRAR EL FOLDER "ejercicios".

rm ejercicios/ -rf


## 28- ABRIR MAUAL DEL COMANDO cat, REVISARLO Y SALIR.

man cat
[]: # (Revisamos y leemos...)
q


## 29- PRACTICAR CON COMANDOS cal, whoami, ping.

cal 2022
whoami
ping www.elperiodico.es


## 30- ATAJOS INTERSANTES Y NO CONOCIDOS ANTES:

[]: # (Ctrl+l equivale a "clear")
[]: # (Ctrl+C+D cierra la terminal)
[]: # (Ctrl+Alt+T abre una terminal)

