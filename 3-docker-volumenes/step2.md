El objetivo de este módulo es demostrar que es posible crear volumenes de forma independiente a los contenedores  

1. Revisión de los volumenes, compruebe que no existe ningún volumen  
`docker volume ls`{{execute}}  

2. Iniciar un contenedor con un nuevo volumen  
`docker run -it --name contenedor1 -v /nuevo-volumen ubuntu`{{execute}}  

3. Salir del contenedor  
`exit`{{execute}}  

4. Revisión de los volumenes, un nuevo volumen fue creado para el contenedor lanzado   
`docker volume ls`{{execute}}  

5. Revisión de los contenedores  
`docker ps -a`{{execute}}  

6. Eliminar el contenedor creado  
`docker rm -f contenedor1`{{execute}}  

Revisión de los volumenes  
7. `docker volume ls`{{execute}}  


Identifique que el volumen creado en el paso  2 no se eliminó a pesar de haber elminado el contenedor con el cual se creó
