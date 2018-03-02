# Introducción a Git

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