
# Sesión 04 - Guardar y Deshacer cambios


## GIT
Elimina un archivo versionado.
Ejemplo: Versionas un archivo y luego lo ignoras en el .gitignore, ese archivo aún sigue versionado a pesar de ser ignorado. Para quitarlo el siguiente comando:
```
git rm --cache <file>
```
fuerza la version de un archivo.
Ejemplo: Versionar un archivo de una carpeta ignorada
```
git add -f <file>
```


Ignora los permisos de archivos y carpetas
```
git config core.fileMode false
```

## GIT SUBMODULE
Clonar un repositorio con submodulos
```
git clone --recursive <url-repo>
```

Actualiza todos los submodulos seteados con el repositorio principal
```
git submodule update --init --recursive
```

Agrega los cambios guardados en el stash al directorio de trabajo
```
git add submodule <url-repo> <submodule-path>
```

Al agregar un submodulo se crea un archivo donde se guradar la relación del repo principal con los submodulos
```
cat .gitmodules
```
Elimina un submodulo del reposiorio pincipal
```
git submodule rm <submodule-path>
```

## GIT BISECT
## GIT REFLOG
## GIT FLOW