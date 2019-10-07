# Como hacer un pull request

## Crear una carpeta nueva
- posicionarse en la carpeta creada y corrrer un git init

## Crear una copia remota del repo
- Forkearlo
- git clone url_de_repositorio_propio


## Crear una nueva rama de trabajo
- git branch nueva-rama
- git checkout nueva-rama
- (atajo) git checkout -b nueva-rama


## Hacer tus cambios locales
- git add .
- git commit -m "mensaje del commit"
- git status
- git push --set-upstream origin nueva-rama


## Configurar repo remoto (repositorio en github)
- git remote -v
- git remote add upstream url_del_repositorio_original


## Sincronizar el Fork con repo local
- git fetch upstream
- git checkout master
- git merge upstream/master


## Mergear al master (local[nuestra computadora])
- git checkout master
- git merge nueva-rama
- git push -u origin master