# Clase 02 - Git Desarrollo Colaborativo

![Git-Github](_ref/git-github.png)

## Repaso de comandos para realizar persistir los cambios de archivos dentro del repositorio

```sh
git status
```

## GIT COMMIT: Para persistir los cambios 
Los archivos elegimos y colocados en el Staging Area vamos a querer persistirlos.

```sh
git commit -m "Mensaje descriptivo de lo que estoy guardando dentro del commit"
```

## Corregir un commit (tanto el mensaje como el contenido)

```sh
git add <nombre-archivo>
git commit --amend
```

## Visualizar el timelime de los commits (instaneas/snapshot)

```sh
git log # versión larga 
git log --oneline # versión corta
git log --oneline -2 # ver una cantidad limitada de commits 
```
Nota: Para salir de la aplicación 'less' tengo que aprentar la tecla 'q' -> quit 

## Hacer commits de parte de un archivo

```sh
git add --patch
# Menú interactivo, donde git me va a ir preguntando que quiero hacer con lo hunks
# y -> Si quiero marcar hunk para enviar al staging area
# n -> No quiero marcar hunk para enviar al staging area
# s -> split -> Le propongo a git que intente hacer la división
# e -> Decido yo que línea quiero enviar al staging area
```

## .gitignore 
Archivo para desestimar diferentes carpetas y archivos que no quiero que formen parte del repositorio

```sh
touch .gitignore
```

## Subiendo nuestro local al remoto

```sh
git remote add <alias> <url>
git remote add origin git@github.com:mlapeducacionit/git-72670.git # Usen HTML
```

## Ver si tengo ya un remoto en mi local

```sh
git remote # Versión corta
git remote -v # Versión detallada
```

## Para subir los cambios

```sh
git push -u <remoto> <rama-local>
git push -u origin main
```

## Para traernos los cambios que sucedieron en el remoto

```sh
git fetch # Me va a traer la metadata actualizada del remoto (.git)
```

## Visualizar una vez hecho eso los ocurrio

```sh
git branch -av
```

```sh
git log --oneline --all
```

```sh
git status
```

## Traerme definitivamente los cambios (commits)

```sh
git pull # Hace un fetch y luego pull
```









