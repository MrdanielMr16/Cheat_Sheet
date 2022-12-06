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
  --> Toma una instantánea del archivo para preparar la versión
- git reset [file]
  --> Mueve el archivo del área de espera, pero preserva su contenido
- git diff
  --> Muestra las diferencias de archivos que no se han enviado aún al área de espera
- git diff --staged
  --> Muestra las diferencias del archivo entre el área de espera y la última versión del archivo
- git commit -m "[descriptive message]"
  --> 
- git branch
- git branch [branch-name]
- git checkout
- git merge [branch]
- git log

## INSPECT & COMPARE
- git log
- git log branchB..branchA
- git log --follow [file]
- git diff branchB...branchA
- git show [SHA]

## SHARE & UPDATE
- git remote add [alias] [url]
- git fetch [alias]
- git merge [alias]/[branch]
- git push [alias] [branch]
- git pull

## TRACKING PATH CHANGES
- git rm [file]
- git mv [existing-path] [new-path]
- git log --stat -M

## REWRITE HISTORY
- git rebase [branch]
- git reset --hard [commit]

## TEMPORARY COMMITS
- git stash
- git stash list
- git stash pop
- git stash drop
