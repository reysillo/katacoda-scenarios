Comandos útiles en docker:  

Revisión la versión de docker que ha sido instalada.  
`docker --version`{{execute}}

## Imágenes  
Descargar una imagen de un registry (DockerHub)  
`docker pull nginx`{{execute}}  

Ver imágenes descargadas o creadas  
`docker images`{{execute}}  

Borrar una imagen  
`docker rmi -f nginx`{{execute}}  

## Contenedores  
Iniciar un contenedor apartir de una imagen (daemon mode)
`docker run -d nginx`{{execute}}

Ver contenedores en ejecución
`docker ps`{{execute}}

Pausar un contenedor
`docker stop [container-id]`{{execute}}

Reinciar un contenedor
`docker start [container-id]`{{execute}}

Detener un contenedor
`docker stop [container-id]`{{execute}}

Ver todos los contenedores del sistema  
`docker ps -a`{{execute}}  

Borrar un contenedor
`docker rm -f [container-id]`{{execute}}