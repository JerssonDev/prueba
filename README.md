# Introducción a Git

## ¿Qué es Git?
Es un sistema de control de versiones para el mantenimiento eficiente y confiable de archivos

## Zonas de Git

1. Working Directory
2. Staging Area
3. Git Directory (Repositorio)

## Flujo de Trabajo

1. Se modifica los archivo en el Proyecto(directorio).
2. Se preparan los archivos añadiendolos al area de preparación.
3. Se confirman los cambios, almacena una copia de los archivos en su estado actual y de manera permanente el el directorio .git

## congiguraciones globales y de inicio en Git

```bash

[mendoza@Jersson ~]$ git config --global user.name "Jersson Mendoza"
[mendoza@Jersson ~]$ git config user.name
Jersson Mendoza
[mendoza@Jersson ~]$ git config --global user.email "jersson926@gmail.com"
[mendoza@Jersson ~]$ git config user.email
jersson926@gmail.com
[mendoza@Jersson ~]$ git config --global core.editor vim
[mendoza@Jersson ~]$ git config core.editor
vim
[mendoza@Jersson ~]$ git config --list
user.name=Jersson Mendoza
user.email=jersson926@gmail.com
core.editor=vim
[mendoza@Jersson ~]$ git config --list | grep user
user.name=Jersson Mendoza
user.email=jersson926@gmail.com
[mendoza@Jersson ~]$ git config --list | grep editor
core.editor=vim
[mendoza@Jersson ~]$ 
```

# Conexion de git con un repositorio en Github

## git remote add origin <"urldelrepo">
te conectas con el repositorio remoto en github
`origin/master` es una rama oculta, una rama del sistema con github, para ver las ramas ocultas ejecutamos `git branch --all`

## pasos para aportar a otro repositorio
1. Hacer un Fork en Github.
2. Clonar el repositorio desde mi cuenta de Github.
3. Crea una rama local con un nombre de preferencia.
4. realizar cambios en la nueva rama local.
5. Confirmar los cambios realizados en local
6. Hacer  push de los cambios (enviar los comits al fork).
7. git push origin <"nombre_rama">
8. crear un pull reuqest con la nueva rama del fork del repositorio en Github 
9. Esperar a que el administrador acepte los cambios del pull request

# Agregada key ssh remote