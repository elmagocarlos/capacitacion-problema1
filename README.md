crear imagen

docker build -t carlos120gt/orbis-training-docker:0.1.0 .

subir imagen

docker login
docker push carlos120gt/orbis-training-docker

cambiar la version

docker tag carlos120gt/orbis-training-docker:0.1.0 carlos120gt/orbis-training-docker:0.2.0

1. �Qu� importancia tiene los tags en un proyecto?
2. �Cu�l es la diferencia entre un tag normal y un tag anotado en git?
3. �C�mo se sube todos los tags de git que hay en mi local?
4. �Es necesario loguearse cada vez que subo una imagen a dockerhub?
5. �Qu� es y para qu� sirve docker?
6. �Cu�l es la diferencia entre docker y VirtualBox (virtualizaci�n)?
7. �Es necesario depender de una imagen de docker base al crear una imagen nueva?
8. �Porqu� debo anteponer el nombre de usuario en una imagen docker nueva?
9. �Que pasa si creo una imagen sin especificar una versi�n o tag, con qu� versi�n se crea?


----------permite ejecutar configurar el puerto 

docker run -d -p "1080:80" carlos120gt/orbis-training-docker:1.0.0

--------Agregar docker-compose para la construcci�n y ejecuci�n de la imagen

docker-compose -f ./docker-compose.yml up

-------- para permitir q se ejecute en segundo plano

 docker-compose -f ./docker-compose.yml up -d

-------- para verificar los LOGs

docker-compose logs

-----------Usando docker run ejecutar npm install

 docker run -w /app -it -v "e:\escritorio carlos\proyecto\Projects\orbis-training-project":/app carlos120gt/orbis-training-docker:2.0.0 npm install














