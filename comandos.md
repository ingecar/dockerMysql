# Verificar version de docker

docker --version

## Descargar una imagen

docker pull mysql:latest

## Listar imágenes

docker image ls

## Borrar imágenes

docker image rm id_imagen

## Crear un contenedor mysql a partir de la imagen

docker run -p 3311:3306 --name Taller -e MYSQL_ROOT_PASSWORD=qwerty -v $PWD/DbTaller:/var/lib/mysql -d mysql

## Listar contenedores

docker container ls
docker ls -al

## Detener contenedor

docker stop id_contenedor

## Borrar un contenedor

docker container rm id_contenedor

## Ejecutar contenedor

docker exec -it Taller mysql -u root -p
