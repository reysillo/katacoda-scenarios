El objetivo de este escenario es desplegar un contenedor a partir de un Dockerfile 

1. Revise que los archivos Dockerfile e index.html se encuentre en la ruta de archivos
`ls`{{execute}}  

2. Revise el contenido del archivo Dockerfile
`cat Dockerfile`{{execute}}  

3. Construcción  de la imagen  
`docker build -t mi-apache:1.0 .`{{execute}}  

4. Ejecución del contenedor exponiendo el puerto 80
`docker run -d -p 80:80 mi-apache:1.0`{{execute}}  

5. Una vez ejecutado el contenedor se puede ver el resultado en el puerto 80 con el siguiente link : https://[[HOST_SUBDOMAIN]]-80-[[KATACODA_HOST]].environments.katacoda.com/  

a