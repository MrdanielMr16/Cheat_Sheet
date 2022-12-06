# **Cheat sheet de Git**

## CONFIGURAR HERRAMIENTAS
Configurar informacion del usuario a nivel global en donde esta informacion se va a mostrar en todos los commits.

- git config --global user.name “[Su nombre]”
  --> Establece su nombre para que aparezcan en todos los commits que usted realice.
- git config --global user.email “[email-valido]”
  --> Establece su email para que al momento de realizar un commit aparezca en la informacion el email que usted registro
- git config --global color.ui auto
  --> Habilita la útil colorización del producto de la línea de comando


## CREAR REPOSITORIOS
Crea un nuevo repositorio o clona uno ya existente.
- git init [project-name] --> Crea un repositorio local con un nombre en especifico.
  --->
- git clone [url] --> Descarga un repositorio existente a traves de una URL.
  -->

## EFECTUAR CAMBIOS
- git status 
  --> Muestra los archivos nuevos o modificados que deben confirmarse.
- git add [file]
  --> Realiza una instancia para una nueva version del archivo o documento.
- git add .
  --> Agrega todos los cambios al siguiente commit. (todos los archivos)
- git reset [file]
  --> Mueve el archivo del área de espera, pero preserva su contenido
- git diff
  --> Muestra los archivos que tienen diferencia y que aun no se han enviado es decir estan en lista de espera.
- git diff --staged
  --> Muestra las diferencias del archivo entre el área de espera y la última versión del archivo
- git commit -m "[descriptive message]"
  --> Confirma los nuevos cambios o la nueva version del archivo junto a un mensaje descriptivo.

## CAMBIOS GRUPALES
- git branch
  --> Muestra todas las ramas que existen en el repositorio actual.
- git branch [branch-name]
  --> Crea una nueva rama con su nombre especifico
- git checkout [branch-name]
  --> Cambia a la rama especificada y actualiza el directorio.
- git merge [branch]
  --> Fusiona el historial de la rama especificada con la rama actual.
- git branch -d [branch-name]
  --> Borra la rama especificada

## NOMBRES DEL ARCHIVO DE REFACTORIZACIÓN
- git rm [file]
  --> Borra el archivo del directorio activo y pone en el área de espera el archivo borrado
- git rm --cached [file]
  --> Retira el archivo del control de versiones, pero preserva el archivo a nivel local
- git mv [file-original] [file-renamed]
  --> Cambia el nombre del archivo y lo prepara para commit
  
  
## SINCRONIZAR CAMBIOS
- git fetch [alias]
  --> Descarga todo el historial del marcador del repositorio
- git merge [alias]/[branch]
  --> Combina la rama del marcador con la rama local actual
- git push [alias] [branch]
  --> Carga todos los commits de la rama local al GitHub
- git pull
  --> Descarga el historial del marcador e incorpora cambios

## REPASAR HISTORIAL
- git log
  --> Enumera el historial de la versión para la rama actual
- git log --follow [file]
  --> Enumera el historial de versión para el archivo, incluidos los cambios
de nombre
- git diff [first-branch]...[second-branch]
  --> Muestra las diferencias de contenido entre dos ramas
- git show [commit]
  --> Produce metadatos y cambios de contenido del commit especificado
  
## REHACER COMMITS
- git reset [commit]
  --> Deshace todos los commits después de [commit], preservando los cambios localmente 
- git reset --hard [commit]
  --> Desecha todo el historial y regresa al commit especificado

## GUARDAR FRAGMENTOS
- git stash
  --> Almacena temporalmente todos los archivos tracked modificados
- git stash list
  --> Enumera todos los sets de cambios en guardado rápido
- git stash pop
  --> Restaura los archivos guardados recientemente
- git stash drop
  --> Elimina el set de cambios en guardado rápido más reciente
