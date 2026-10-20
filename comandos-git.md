# Comandos de Git

## Empezar
- `git init` = sirve para iniciar un repositorio en la carpeta
- `git status` = muestra cómo están los archivos (nuevos, modificados o listos para commit)
- `git status --short` = lo mismo pero resumido

## Guardar cambios
- `git add archivo` = agrega un archivo para el siguiente commit
- `git add .` = agrega todos los archivos
- `git commit` = abre Vim para escribir el mensaje (`i` para escribir, `Esc` y `:wq` para guardar y salir)
- `git commit -m "mensaje"` = guarda los cambios con un mensaje
- `git commit -am "mensaje"` = agrega los archivos modificados y hace el commit de una vez

## Ver historial
- `git log` = muestra todos los commits
- `git log --oneline` = muestra los commits en una sola línea
- `git log --stat` = muestra los commits y qué archivos cambiaron en cada uno
- `git log --oneline --graph --all` = muestra el dibujo de las ramas y los merges
- `git show` = muestra los cambios del último commit
- `git diff` = muestra los cambios que aún no tienen commit
- `git diff commit1 commit2` = compara dos commits

## Moverse en el historial
- `git checkout id-del-commit` = viaja a un commit anterior para verlo
- `git checkout master` = regresa al último commit de la rama

## Ramas
- `git branch` = muestra las ramas
- `git branch nombre` = crea una rama nueva
- `git checkout nombre` = cambia a otra rama
- `git switch nombre` = también cambia a otra rama (forma nueva)
- `git switch -c nombre` = crea la rama y se cambia a ella de una vez
- `git branch -d nombre` = borra una rama que ya se unió

## Merge
- `git merge nombre` = une la rama indicada con la rama donde estoy
- `git merge --abort` = cancela el merge si hay conflicto y deja todo como estaba
- Conflicto = cuando las dos ramas cambian la misma línea; se arregla eligiendo qué dejar entre `<<<<<<<`, `=======` y `>>>>>>>` y haciendo commit

## GitHub
- `git branch -M main` = cambia el nombre de la rama master a main
- `git remote add origin url` = conecta el repositorio con GitHub
- `git push -u origin main` = sube los cambios a GitHub
- `git push origin nombre` = sube otra rama a GitHub
- `git clone url` = descarga un repositorio de GitHub a mi PC
- `git fetch` = revisa si hay cambios nuevos en GitHub sin unirlos
- `git pull` = trae los cambios de GitHub a mi PC

## Terminal
- `ls -al` = muestra los archivos de la carpeta, incluso los ocultos como `.git`
- `clear` = limpia la pantalla
- `history` = muestra los comandos que he usado
