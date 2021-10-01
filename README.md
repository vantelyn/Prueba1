# Guía básica Git + Github

&ensp;   
## Índice
1. **Descarga e instalación de GIT**
    1. Windows
    1. Linux
2. **Primeros pasos**
    1. Windows vs Linux
    2. Registro de credenciales
3. **Uso de repositorios**
    1. Crear repositorio local
    2. Clonar repositorio remoto
    3. Inicializar el control de versiones
4. **Iniciación a Github**
    1. Crear una nueva cuenta
    1. Generación Token de autentificación
    1. Crear nuevo repositorio (online)
    1. Enlazar repositorios 
5. **Proyectos de grupo**
    1. Cómo invitar a un colaborador
    2. Unirse a un proyecto existente
    3. Resolución de conflictos
6. **Guía completa de instrucciones**

&ensp;  
## 1. Descarga e instalación de GIT

### &ensp;1.1. En Windows
* Descargar el instalador de la web oficial:
```
https://git-scm.com/download/win
```
* Ejecutar y seguir las instrucciones del instalador.

### &ensp;1.2. En Linux (Ubuntu)
&emsp;En Ubuntu se recomiendan las siguientes instrucciones en consola:

* Comprobar la versión instalada:
```
$ git --version
```
* Actualizar índice local de paquetes:
```
$ sudo apt update
```
* Instalar GIT:
```
$ sudo apt install git
```
&nbsp;  
&emsp;Para otras versiones de linux visitar la página de descarga oficial:
```
https://git-scm.com/download/linux
```

&emsp;

## 2. Primeros pasos
### &ensp;2.1. Windows vs Linux
* En **Linux** Git se utiliza mediante una serie de instrucciones ejecutables desde la terminal, todas de ellas empezando por git:

![Foto Git Bash Windows](https://github.com/vantelyn/Prueba1/blob/master/cmdLinux.jpg "Linux")

* En **Windows** Git se puede utilizar tanto mediante su interfaz gráfica -**Git GUI**-, cómo mediante la línea de commandos -**Git CMD/Git Bash**-. Estas opciones son accesibles bien desde el buscador de Windows o haciendo click derecho en el escritorio o la carpeta de trabajo.  
&ensp;  
A efectos de esta guía vamos a utilizar Git Bash dado que emula la consola de comandos de Linux:
  
![Foto Git Bash Windows](https://github.com/vantelyn/Prueba1/blob/master/bashWindows.jpg "Windows")

### &ensp;2.2. Registro de credenciales
Antes de poder hacer uso de las funciones de Git es obligatorio configurar las credenciales con las que vamos a firmar nuestro trabajo. Para ello vamos a hacer uso de las siguientes instrucciones:
* **Registrar nombre:**
```
$ git config --global user.name "John Doe"
```
* **Registrar dirección de correo electrónico:**
```
$ git config --global user.email johndoe@example.com
```
&ensp;  

## 3. Uso de repositorios
### &emsp;3.1. Crear repositorio local
La manera más simple de crear un repositorio es transformando una carpeta de archivos local en un repositorio de trabajo. Si dispones de un proyecto cuyo control de versiones no está implementado aún y quieres empezar a controlarlo con Git, deberás seguir los siguientes pasos:
* **Desplazar el terminal hasta carpeta de trabajo:**

&emsp;En Linux
```
$ cd /home/user/my_project
```
&emsp;En Windows
```
$ cd C:/Users/user/my_project
```
&emsp;Esto también se puede hacer abriendo directamente el terminal desde la misma carpeta.

* **Inicializar Git**

&emsp;Una vez situados dentro del directorio del proyecto podemos inicializar el control de versiones Git mediante la siguiente instrucción:
```
$ git init
```
Esta instrucción crearía un nuevo subdirectorio oculto nombrado `.git` que contiene todos los archivos necesarios para el funcionamiento del repositorio.
### &emsp;3.2. Clonar repositorio remoto
Si por lo contrario quieres trabajar con un repositorio ya existente, como por ejemplo un proyecto de grupo en el que estás participando, la instrucción a utilizar sería `git clone` seguido de la `<url>` donde se ubica dicho proyecto.

&emsp;Por ejemplo:
```
$ git clone https://github.com/libgit2/libgit2 [nombreProyecto]
```
Esta instrucción crearía -dentro del directorio activo del usuario- una nueva carpeta con el nombre del proyecto, la cual contendría una copia de todos los archivos almacenados en el servidor -incluídas sus versiones anteriores-.

### &emsp;3.3. Inicializar el control de versiones

&ensp;  
## 4. Iniciación a Github
### &emsp;4.1. Crear una nueva cuenta
### &emsp;4.2. Generación Token de autentificación
### &emsp;4.3. Crear repositorio Github
### &emsp;4.4. Enlazar repositorios
&ensp;  
## 5. Proyectos de grupo
### &emsp;5.1. Cómo invitar a un colaborador
### &emsp;5.2. Unirse a un proyecto existente
### &emsp;5.3. Resolución de conflictos
&ensp;  
## 6. Guía completa de instrucciones
