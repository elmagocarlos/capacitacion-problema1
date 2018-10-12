crear imagen

docker build -t carlos120gt/orbis-training-docker:0.1.0 .

subir imagen

docker login
docker push carlos120gt/orbis-training-docker

cambiar la version

docker tag carlos120gt/orbis-training-docker:0.1.0 carlos120gt/orbis-training-docker:0.2.0

1. ¿Qué importancia tiene los tags en un proyecto?
2. ¿Cuál es la diferencia entre un tag normal y un tag anotado en git?
3. ¿Cómo se sube todos los tags de git que hay en mi local?
4. ¿Es necesario loguearse cada vez que subo una imagen a dockerhub?
5. ¿Qué es y para qué sirve docker?
6. ¿Cuál es la diferencia entre docker y VirtualBox (virtualización)?
7. ¿Es necesario depender de una imagen de docker base al crear una imagen nueva?
8. ¿Porqué debo anteponer el nombre de usuario en una imagen docker nueva?
9. ¿Que pasa si creo una imagen sin especificar una versión o tag, con qué versión se crea?


----------permite ejecutar configurar el puerto 

docker run -d -p "1080:80" carlos120gt/orbis-training-docker:1.0.0



--------Agregar docker-compose para la construcción y ejecución de la imagen

docker-compose -f ./docker-compose.yml up

-------- para permitir q se ejecute en segundo plano

 docker-compose -f ./docker-compose.yml up -d

-------- para verificar los LOGs

docker-compose logs

-----------Usando docker run ejecutar npm install

 docker run -w /app -it -v "e:\escritorio carlos\proyecto\Projects\orbis-training-project":/app carlos120gt/orbis-training-docker:2.0.0 npm install

7. Exponer los puertos 3030 y 35729 en la imagen de docker, luego ejecutar npm start usando docker run

docker run -p "35729:3030" -p "3030:3030" -w /app -v  "e:\escritorio carl
os\proyecto\Projects\orbis-training-project":/app  carlos120gt/orbis-training-docker:2.0.0 npm start


10. Usando la imagen de docker, ejecutar npm run release

docker run -p "35729:1042" -w /app -v  "e:\escritorio carlos\proyecto\Projects\orbis-training-project":/app  carlos120gt/orbis-training-docker:2.0.0 npm rum release















