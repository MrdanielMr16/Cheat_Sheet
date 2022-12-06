# **Cheat sheet de Git**

## CONFIGURAR HERRAMIENTAS

- git config --global user.name “[Su nombre]”
   --> Establece su nombre para que aparezcan en todos los comits que usted realice.
- git config --global user.email “[email-valido]”
    Establece su email para que al momento de realizar un comit aparezca en la informacion el email que usted registro
- git config --global color.ui auto
    Habilita la útil colorización del producto de la línea de comando


## Setup & Init

- git init
- git clone [url]

## BRANCH & MERGE

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
