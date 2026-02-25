## Configuración Básica

Configurar Nombre que salen en los commits
```ssh
	git config --global user.name "dasdo"
```
Configurar Email
```ssh	
	git config --global user.email dasdo1@gmail.com
```
Marco de colores para los comando
```ssh
	git config --global color.ui true
```

## Iniciando repositorio

Iniciamos GIT en la carpeta donde esta el proyecto
```ssh
	git init
```
Clonamos el repositorio de github o bitbucket
```ssh
	git clone <url>
```
Añadimos todos los archivos para el commit
```ssh
	git add .
```
Hacemos el primer commit
```ssh
	git commit -m "Texto que identifique por que se hizo el commit"
```
subimos al repositorio
```ssh
	git push origin master
```

## GIT CLONE


Clonamos el repositorio de github o bitbucket
```ssh
	git clone <url>
```
Clonamos el repositorio de github o bitbucket ?????
```ssh
	git clone <url> git-demo
```

## GIT ADD


Añadimos todos los archivos para el commit
```ssh
	git add .
```
Añadimos el archivo para el commit
```ssh
	git add <archivo>
```
Añadimos todos los archivos para el commit omitiendo los nuevos
```ssh
	git add --all 
```
Añadimos todos los archivos con la extensión especificada
```ssh
	git add *.txt
```
Añadimos todos los archivos dentro de un directorio y de una extensión especifica
```ssh
	git add docs/*.txt
```
Añadimos todos los archivos dentro de un directorios
```ssh
	git add docs/
```
## GIT COMMIT

Cargar en el HEAD los cambios realizados
```ssh
	git commit -m "Texto que identifique por que se hizo el commit"
```
Agregar y Cargar en el HEAD los cambios realizados
```ssh
	git commit -a -m "Texto que identifique por que se hizo el commit"
```
De haber conflictos los muestra
```ssh
	git commit -a 
```
Agregar al ultimo commit, este no se muestra como un nuevo commit en los logs. Se puede especificar un nuevo mensaje
```ssh
	git commit --amend -m "Texto que identifique por que se hizo el commit"
```
## GIT PUSH

Subimos al repositorio
```ssh
	git push <origien> <branch>
```
Subimos un tag
```ssh
	git push --tags
```
## GIT LOG

Muestra los logs de los commits
```ssh
	git log
```
Muestras los cambios en los commits
```ssh
	git log --oneline --stat
```
Muestra graficos de los commits
```ssh
	git log --oneline --graph
```
## GIT DIFF

Muestra los cambios realizados a un archivo
```ssh
	git diff
	git diff --staged
```
## GIT HEAD

Saca un archivo del commit
```ssh
	git reset HEAD <archivo>
```
Devuelve el ultimo commit que se hizo y pone los cambios en staging
```ssh
	git reset --soft HEAD^
```
Devuelve el ultimo commit y todos los cambios
```ssh
	git reset --hard HEAD^
```
Devuelve los 2 ultimo commit y todos los cambios
```ssh
	git reset --hard HEAD^^
```
Rollback merge/commit
```ssh
	git log
	git reset --hard <commit_sha>
```
## GIT REMOTE

Agregar repositorio remoto
```ssh
	git remote add origin <url>
```
Cambiar de remote
```ssh
	git remote set-url origin <url>
```
Remover repositorio
```ssh
	git remote rm <name/origin>
```
Muestra lista repositorios
```ssh
	git remote -v
```
Muestra los branches remotos
```ssh	
	git remote show origin
```
Limpiar todos los branches eliminados
```ssh
	git remote prune origin 
```
## GIT BRANCH

Crea un branch
```ssh
	git branch <nameBranch>
```
Lista los branches
```ssh
	git branch
```
Comando -d elimina el branch y lo une al master
```ssh
	git branch -d <nameBranch>
```
Elimina sin preguntar
```ssh
	git branch -D <nameBranch>
