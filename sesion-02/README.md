
# Sesión 02 - Ramificaciones y Fusiones

## GIT BRANCH
Lista todas las ramas locales

```
git branch
```
Lista todas las ramas locales y remotas descargadas

```
git branch -a
```
Crea una rama

```
git branch <branch_name>
```
Borra una rama especifica que este fusionada (Nos ayuda a validar, que la rama que vamos a borrar no tenga nada nuevo)

```
git branch -d <branch_name>
```
Borra una rama especifica de manera forzada (Sin advertencias)

```
git branch -D <branch_name>
```

Renombrar rama o cambiar de nombre a una rama

```
git branch -m <branch_name> <new_branch_name>
```
Lista todas las ramas que no se han combinado

```
git branch --no-merged / git branch --no-merged master

```
Para enumerar las confirmaciones relevantes:

```
git cherry -v master <branch>
```
## GIT CHECKOUT
Cambia de commit o rama

```
git checkout <hash_commit/branch_name>

```
Crea una rama y nos mueve a ella
```
git checkout -b <branch_name>
```
## GIT FETCH
Descarga todas las ramas remotas

```
git fetch --all
```
Descarga una rama especifica

```
git fetch <branch_name>
```
## GIT MERGE
```
git merge <branch_name>
```
## GIT PUSH
Subimos los archivos al repositorio de manera forzada reescribiendo la historia

```
git push origin +<branch_name>
```
## GIT IGNORE
Ignora archivos del repositorio en el archivo .gitignore

```
git push origin +<branch_name>
```
## GIT TAG
Etiquetas y versiones “banderas”. (git tag)

```
git tag <tag_name>
```
Sube todos los tags locales al repositorio remoto

```
git push --tags
```
```
git tag -a 1.0.0
```
```
git tag -l "1.0.*"
```
```
git show -a 1.0.0
```

## GIT REBASE
Reescribir la historia del proyecto
```
git rebase
```