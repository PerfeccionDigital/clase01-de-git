
## Comandos útiles para la terminal

Lista el contenido de un directorio
```
ls
```
Lista el contenido mostrando fecha y hora
```
ls -l
```
Mostrar en qué carpeta estoy trabajando
```
pwd
```
Crear directorio
```
mkdir nombre_directorio
```
Entrar en directorio (cambiar de directorio)
```
cd
```
Salir del directorio (cambia al directorio anterior)
```
cd ..
```
Crear directorio
```
mkdir nombre_directorio
```
Borrar directorio con contenido
```
rm -Rf nombre_directorio
```
Mostrar todo el contenido de un archivo (sólo hacerlo con archivos de texto)
```
cat nombre_archivo
```
Crea un archivo
```
touch nombre_archivo
```
Abre el editor Vim
```
vim nombre_archivo
```






## Configuración Básica

Configurar Nombre que salen en los commits
```
git config --global user.name "Nomnbre del Usuario"
```
Configurar Email
```
git config --global user.email usuario@gmail.com
```
Marco de colores para los comando
```
git config --global color.ui true
```

## Iniciando repositorio

Iniciamos GIT en la carpeta donde esta el proyecto
```
git init
```
Añadimos todos los archivos para el commit
```
git add .
```
Hacemos el primer commit
```
git commit -m "El mensaje del commit tiene que ser muy descriptivo"
```
subimos al repositorio
```
git push origin master
```

## GIT CLONE

Clonamos un repositorio por htts o ssh
```
git clone <url>
```

## GIT STATUS

Muestra el estado de los archivos modificados o agregados
```
git status
```

## GIT ADD

Añadimos todos los archivos para el commit
```
git add .
```
Añadimos un archivo específico para el commit
```
git add <archivo>
```
Añadimos todos los archivos para el commit omitiendo los nuevos
```
git add --all
```
Añadimos todos los archivos con la extensión especificada
```
git add *.txt
```
## GIT COMMIT

Cargar en el HEAD los cambios realizados
```
git commit -m "Mensaje que identifique por que se hizo el commit"
```
Agregar y Cargar en el HEAD los cambios realizados
```
git commit -am "Mensaje que identifique por que se hizo el commit"
```
Modifica el mensaje del último commit
```
git commit --amend -m "Mensaje que identifique por que se hizo el commit"
```
## GIT PUSH

Subimos al repositorio
```
git push <origien> <branch>
```
## GIT LOG

Muestra los logs de los commits
```
git log
```
Muestra una lista de archivos por cada commit
```
git log --name-status
```
## GIT DIFF

Muestra los cambios realizados a un archivo
```
git diff
git diff <archivo>
```
## GIT RESET

Saca los archivos agregados al staging area
```
git reset
```
## GIT REMOTE

Agregar repositorio remoto
```
git remote add origin <url>
```
Cambiar de remote
```
git remote set-url origin <url>
```
Remover repositorio
```
git remote rm <name/origin>
```
Muestra lista repositorios
```
git remote -v
```
## CIT CHECKOUT


Quita del HEAD un archivo y le pone el estado de no trabajado
```
git checkout <file>
```
Crea un branch en base a uno online
```
git checkout -b newlocalbranchname origin/branch-name
```

