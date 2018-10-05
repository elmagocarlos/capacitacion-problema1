crear imagen

docker build -t carlos120gt/orbis-training-docker:0.1.0 .

subir imagen

docker login
docker push carlos120gt/orbis-training-docker

cambiar la version

docker tag carlos120gt/orbis-training-docker:0.1.0 carlos120gt/orbis-training-docker:0.2.0


