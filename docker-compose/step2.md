## Crear un volumen al vuelo 
1. Revisión de los volumenes  
`docker volume ls`{{execute}}  

2. Iniciar un contenedor con un nuevo volumen
`docker run -it --name contenedor1 -v /nuevo-volumen ubuntu`{{execute}}  

3. Salir del contenedor Crtl+c

4. Revisión de los volumenes  
`docker volume ls`{{execute}}  

5. Revisión de los contenedores
`docker ps -a`{{execute}}  

6. Eliminar el contenedor creado
`docker rm -f contenedor1`{{execute}}  

Revisión de los volumenes  
7. `docker volume ls`{{execute}}  
