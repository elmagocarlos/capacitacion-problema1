# Ejercicio 1

Capacitacion: Git, bash y docker

Integrantes:

- Jose Clemente

- Carlos Gomez

- Scrum Master: Carlos Gomez

## 1�Qu� es y para qu� sirve GIT?
Es un sistema de control de versiones.

## 2�Que es Github o bitbucket?
Es un servicio en la nube que ayuda a los desarrolladores a almacenar y administrar su c�digo.

## 3�Qu� es y para qu� sirve el SSH?
Es un protocolo para acceder de forma remota a un servidor privado

## 4�Que pasa si cambio de PC? �Tendr� que generar el SSH nuevamente?�Por qu�?
Si cambio de maquina debe configurar nuevamnete SSH, razon por al cual se debera generr nuevamnte el SSH, debido a que el key es unico por PC.


## 5�Qu� es markdown? �Para qu� sirve?
Markdown es un lenguaje de marcado que facilita la aplicaci�n de formato a un texto empleando una serie de caracteres de una forma especial y sirve para convierte el lenguaje en HTML v�lido.

## 7�C�mo inicializo y configuro un proyecto de git?
iniciar
```sh
$ git config --global user.email "you@example.com"
$ git config --global user.name "Your Name"
```
configurar
```sh
$ git init
```

# git stash

## 1. �Para qu� ayuda el `git stash`?
Permite guardar datos en memoria

## 2. �Cu�l es la diferencia entre `git stash pop` y `git stash apply`?
git stash pop remueve el escondite despu�s de aplicarlo, mientras que lo git stash apply deja en la lista oculta para su posible reutilizaci�n posterior .

## 3. �Qu� significa el modo interactivo del `git rebase`?
Git rebase b�sicamente lo que hace es recopilar uno a uno los cambios confirmados en una rama, y reaplicarlos sobre otra. Utilizar rebase nos puede ayudar a evitar conflictos siempre que se aplique sobre commits que est�n en local y no han sido subidos a ning�n repositorio remoto

## 4. �Cual es la diferencia entre la shell y la terminal?
Terminal = Entorno de entrada y salida
Shell = interprete de linea de comendos

## 5. �Que hace estos comandos? `git clone`, `git status`, `git add`, `git commit`, `git push`, `git checkout`, `git stash`, `git rebase`, `git merge`, `git branch`, `git push`,

git clone:Clona un proyecto de git en la carpeta NombreProyecto.
git status:Nos indica el estado del repositorio, por ejemplo cuales est�n modificados, cuales no est�n siendo seguidos por GIT, entre otras caracter�sticas
git add:Agrega al repositorio los archivos que indiquemos.
git commit:Hace commit a los archivos que indiquemos, de esta manera quedan guardados nuestras modificaciones
git push:Luego de que hicimos un git commit, si estamos trabajando remotamente, este comando va a subir los archivos al repositorio remoto, espec�ficamente al branch que indiquemos
git checkout:Crea un nuevo branch y automaticamente GIT se cambia al branch creado, clonando el branch desde donde ejecutamos el comando
git stash:Permite guardar datos en memoria
git rebase:�sicamente lo que hace es recopilar uno a uno los cambios confirmados en una rama, y reaplicarlos sobre otra
git merge:Hace un merge entre dos branches, en este caso la direcci�n del merge ser�a entre el branch que indiquemos en el comando, y el branch donde est�mos ubicados
git branch:Nos muestra una lista de los branches que existen en nuestro repositorio
git push:Hace una actualizaci�n en nuestro branch local, desde un branch remoto que indicamos en el comando.


























