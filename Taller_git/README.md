# Taller_git
Repositorio de taller 1 en git bash, estudiante 

Inicialmente se ingresa a la cuenta de github
- se crea un nuevo Repositorio
- añadido con nombre Taller_git
- desde la consola de bash se abre una terminal
- se crea con el comando mkdir la carpeta Taller_git
- se accede a la carpeta con cd
1. Configuracion inicial
- se inicializa el repositorio con el comando git init Taller_git
- se configura el nombre y email del git
- con git config list se puede corroborar

2. Ramas
- se crea la rama feature
- se crea un archivo en dicha rama
- se agrega y hacemos el primer commit
- con echo se crea o edita el archivo ya creado
- se hace un segundo commit
En pocas palabras se editó el archivo que creamos

3. Merge y Rebase
- volvemos a la rama master
- se mergea la rama feature con la rama master
- los archivos de feature ahora estan en master
- se enlista los commits con el comando git log --oneline
- se copia el hash del ultimo commit
- con el comando git reset --hard <y el hash del commit>
se accede a una version previa al mergea
- se revierte el merge por medio de Rebase
- la rama rebase esta de nuevo

4- cherry pick reflog
- se crea la rama hotfix
- creacion de archivo.txt
- se hace un commit
- se regresa a master
- se le hace un cherry pick a la rama hotfix
- para acceder al historial de commit se usa git reflog, o git log --oneline 
-> ambos sirven para ver el historial de commits, el hash y la descripcion

5. Gestion de conflictos
- se crea la rama feature
- creacion de archivo conflicto.txt
- se hace un commit
- se regresa a la rama master
- se crea el archivo conflicto.txt
- se hace un commit desde esa rama
- se hace el merge
- se muestra el conflicto (master | merging)
- se debe acceder al archivo conflicto.txt y eliminar los elementos que están en conflicto
- se añade y se hace un commit
- la rama recupera su estado (master)

6. Conexion a git hub
- se enlaza ambos proyectos a traves del comando git remote y la url 
- es necesario hacer un fetch 
- se crea la rama main y se hace merge a master
- se hace un push
