
# Sesión 03 - Guardar y Deshacer cambios



## Ejercicio


Temas nuevos:
* git stash
* git clean
* git reset
* git cherry-pick
* git revert
* git log grep

## GIT STASH

Guarda todos los archivos modificados y nuevos
```
git stash --include-untracked
```
Lista los archivos modificados
```
git stash show --name-only
```
#### Diferencia entre el HEAD y el stash
Muestra la diferencia de tu rama actual con un stash
```
git diff master stash@{0}
git diff HEAD stash@{0}
git diff stash@{0}^!
```
Muestra los archivos modificados entre una rama y un stash

#### Comprar un archivo especifico del stash
```
git diff --name-only stash
git diff --name-only stash@{0} master
```
lista la diferencia de un archivo en stash
```
 git  diff develop..stash@{0} classes/PaymentModule.php
```
#### Recuperar un archivo especifico del stash

Recupera un archivo especifico y lo aplica en working direcory
```
git show stash@{0}:MyFile.txt > MyFile.txt
```

Recupera un archivo especifico y lo manda al staging area
```
git checkout stash login.html v2.html
```

## GIT HELP


Cuenta la cantidad de commits
```
git rev-list --count maste
```
Cuenta la diferencia de commits de donde estas con la rama a comprar
```
git rev-list --count HEAD ^master
```
Lista la cantidad de commits por usuario
```
git shortlog -s -n
```
Contar commits por un rango de fechas
```
git shortlog -sne --since="01 Jan 2015" --before="01 Feb 2015"
```

```
git log --oneline master..develop
```

```
git log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr)%Creset' --abbrev-commit --date=relative master..develop
```

## GIT LOG
```
git log --grep "etiqueta"
```