# Guía básica Git más Github
***
&ensp;   
## Índice
1. **Descarga e instalación de GIT**
    1. Windows
    1. Linux
1. **Primeros pasos**
    1. Windows vs Linux
    1. Registro de credenciales
1. **Uso de repositorios**
    1. Crear repositorio local
    1. Clonar repositorio remoto
    1. Inicializar el control de versiones
1. **Iniciación a Github**
    1. Crear una nueva cuenta
    1. Generación Token de autentificación
    1. Crear nuevo repositorio (online)
    1. Enlazar repositorios 
1. **Proyectos de grupo**
    1. Cómo invitar a un colaborador
    1. Unirse a un proyecto existente
    1. Resolución de conflictos
1. **Guía completa de instrucciones**
1. **Conclusión**
1. **Bibliografía**

&ensp;  
## 1. Descarga e instalación de GIT

### 1.1. En Windows
* **Descargar** el instalador de la web oficial:
    ```
    https://git-scm.com/download/win
    ```
* Ejecutamos el instalador y seguimos las instrucciones.

### 1.2. En Linux (Ubuntu)
En **Ubuntu** se recomiendan las siguientes instrucciones en consola:

* **Comprobar** si hay alguna versión instalada:
    ```
    $ git --version
    ```
* **Actualizar** índice local de paquetes:
    ```
    $ sudo apt update
    ```
* **Instalar** GIT:
    ```
    $ sudo apt install git
    ```
&nbsp;  
Para **otras versiones de linux** puedes visitar la página de descarga oficial:
```
https://git-scm.com/download/linux
```
&emsp;
## 2. Primeros pasos
### 2.1. Windows vs Linux
* **Linux**
    En Linux **Git se utiliza** mediante una serie de instrucciones ejecutables **desde la terminal**:

    ![Foto Git Bash Windows](https://raw.githubusercontent.com/vantelyn/Prueba1/master/cmdLinux.jpg "Linux")

* **Windows**
    En Windows Git se puede utilizar tanto mediante su interfaz gráfica -**Git GUI**-, cómo mediante la línea de commandos -**Git CMD/Git Bash**-. Estas opciones son accesibles bien desde el buscador de Windows o haciendo click derecho en el escritorio o la carpeta de trabajo. 
&ensp;  
A efectos de esta guía vamos a utilizar Git Bash dado que emula la consola de comandos de Linux:
  
    ![Foto Git Bash Windows](https://raw.githubusercontent.com/vantelyn/Prueba1/master/bashWindows.jpg "Windows")

### 2.2. Registro de credenciales
Es obligatorio **configurar nuestras credenciales** antes de utilizar Git:
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
### 3.1. Crear un repositorio local

* **Desplazar la terminal hasta la carpeta de trabajo:**

    En **Linux**
    ```
    $ cd /home/user/my_project
    ```
    En **Windows**
    ```
    $ cd C:/Users/user/my_project
    ```

* **Inicializar Git**

    Una vez situados dentro del directorio del proyecto podemos inicializar el control de versiones Git mediante la siguiente instrucción:
    ```
    $ git init
    ```
### 3.2. Clonar repositorio remoto
Para **clonar un repositorio ya existente** la instrucción a utilizar sería `git clone` seguido de la `<url>` donde se ubica el repositorio:
```
$ git clone https://github.com/usuario/nombreRepositorio
```
### 3.3. Inicializar el control de versiones
* Puesta en **seguimiento:**
  
    **Añadir un archivo** a la lista de seguimiento:
    ```
    $ git add "nombreArchivo"
    ```
    **Añadir todos los archivos** a la lista de seguimiento:
    ```
    $ git add .
    ```
* **Guardado:**
  
    Para **guardar todos los cambios** realizados en los archivos en seguimiento:
    ```
    $ git commit -m 'First Commit'
    ```
&ensp;
## 4. Iniciación a Github
### 4.1. Crear una nueva cuenta
* **Abrimos la página web de GitHub** en nuestro explorador:
    ```
    https://github.com/
    ```
* Sign up
* Correo electrónico, contraseña y nombre de usuario
* Confirmar correo electrónico
### 4.2. Generación de Token de autentificación
```
Settings > Developer Settings > Personal Access Tokens > Generate new token > Generate token > Copiar el token
```
### 4.3. Crear un repositorio GitHub
```
New Repository > Repository Name > Add a README file (opcional)
```
### 4.4. Subir un repositorio local a GitHub
* Crear repositorio local:
    ```
    git init
    git add "nombreArchivo"
    git commit -m "first commit"
    ```
* Enlazar el repositorio local con el repositorio GitHub
    ```
    git remote add origin https://github.com/usuario/nombreRepositorio.git
    git branch -M main
    git push -u origin main
    ```
&ensp;  
## 5. Proyectos de grupo
### 5.1. Cómo invitar a un colaborador
```
repositorio > Settings > Manage access > Add people > usuario a invitar
```
### 5.2. Unirse a un proyecto existente
```
correo > View invitation > Accept invitation
```
### 5.3. Resolución de conflictos de unión
```
repositorio > Pull requests > Resolve conflicts
```
`<<<<<<` `======` `>>>>>>`

```
Mark as resolved > Commit merge > Pick branch
```
&ensp;  
## 6. Guía completa de instrucciones
## 7. Conclusiones
## 8. Bibliografía
[Resolución de conflictos](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-on-github)
