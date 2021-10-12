# Ejercicio 1: Bash Scripting


&ensp;
## 1. CREAR UNA CARPETA PARA REALIZAR EL EJERCICIO

  ### 1.1 Abrimos terminal

  ### 1.2 Navegamos al área de trabajo

```
   cd $HOME/Desktop
```

  ### 1.3 Creamos una carpeta para el ejercicio

```
   mkdir Ejercicio
```

   ### 1.4 Navegamos a la carpeta que acabamos de crear

```
   cd Ejercicio/
```
&ensp;  

## 2. CREAR UN SCRIPT DE BASH QUE CREE UNA CAREPTA EN LA QUE SE INCLUYA UNA [PLANTILLA WEB RESPONSIVE](http://getskeleton.com/)  

   ### 2.1 Creamos un archivo .sh (archivo Bash)

```
   touch script.sh
```
   ### 2.2 Abrimos el archivo con el editor de texto *Gedit* como proceso hijo

```
   gedit script.sh &
```

   ### 2.3 Dentro del editor, en la primera línea declaramos el archivo como script de *Bash* mediante la siguiente instrucción:

```bash
   #!/bin/bash
```

   ### 2.4 Añadimos una declaración *if* para comprobar si el usuario ha introducido el nombre de la carpeta como argumento de entrada:

```bash
      #!/bin/bash
                     #  4.1 COMPROBAMOS SI EL NÚMERO TOTAL DE ARGUMENTOS INTRODUCIDOS ES MAYOR QUE 0:
      if [ $# -gt 0 ];
      	then
                     #  4.2 EN CASO CONTRARIO GENERAMOS UN MENSAJE DE ERROR Y EL CÓDIGO DE SALIDA CORRESPONDIENTE:
      	else	         
      		echo "Nombre de la carpeta no especificado";
      		exit 1
      fi
```

   ### 2.5 Cuando se cumpla la condición  especificada en el *if*:

```bash
      #!/bin/bash
      if [ $# -gt 0 ];
      	then
      		#  5.1 CREAMOS UNA NUEVA VARIABLE Y LE ASIGNAMOS EL MISMO VALOR QUE EL PRIMER ARGUMENTO DE ENTRADA ($1):
      		nomCarpeta = $1
      		#  5.2 CREAMOS UNA NUEVA CARPETA CON DICHO VALOR COMO NOMBRE:
      		mkdir -p "$nomCarpeta"
      		#  5.3 NAVEGAMOS A LA CARPETA QUE ACABAMOS DE CREAR:
      		cd $nomCarpeta
      		#  5.4 DESCARGAMOS LA PLANTILLA WEB RESPONSIVE:
      		wget https://github.com/dhg/Skeleton/releases/download/2.0.4/Skeleton-2.0.4.zip
      		#  5.5 DESCOMPRIMIMOS SU CONTENIDO:
      		unzip Skeleton-2.0.4.zip
      		#  5.6 MOVEMOS TODOS LOS FICHEROS DE LA CARPETA Skeleton-2.0.4 A LA CARPETA MADRE:
      		mv Skeleton-2.0.4/* .
      		#  5.7 ELIMINAMOS LA CARPETA Skeleton-2.0.4
      		rm -R Skeleton-2.0.4/
      		#  5.8 ELIMINAMOS EL FICHERO Skeleton-2.0.4.zip
      		rm Skeleton-2.0.4.zip
      		#  5.9 INDICAMOS QUE EL PROGRAMA HA FINALIZADO CON ÉXITO:
      		exit 0
      	else
      		echo "Nombre de la carpeta no especificado";
      fi
```
&ensp;        

## 3. Ejecutar el script y comprobar que funciona
