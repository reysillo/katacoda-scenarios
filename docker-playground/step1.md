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

---
## Correr código en un contendor en ejecución

Ejecución de un contenedor  
`docker run ubuntu`{{execute}}  

Modo interactivo (-i), obtener la entrada y la salida estándar del terminal TTY (-t)  
`docker run -it ubuntu`{{execute}}  

Identifique la versión del kernel de la distribución de Oracle Linux  
`docker run -it oraclelinux`{{execute}}  

Verifique la versión del sistema operativo actual  
`cat /etc/*-release`{{execute}}  

Ejecución de código al arranque del contenedor  
`docker run ubuntu ls`{{execute}}  