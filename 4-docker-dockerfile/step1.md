
## Creación de imágenes Docker
1. Ingrese a la carpeta demo  
`cd demo`{{execute}}  

2. Revisión del contenidos  
`ls`{{execute}}    
`cat Dockerfile`{{execute}}  

3. Construcción  de la imagen  
`docker build -t mi-apache:1.0 .`{{execute}}  

4. Ejecución del contenedor  
`docker run -d  -p 80:80 mi-apache:1.0`{{execute}}  

5. Una vez ejecutado el contenedor se puede ver el resultado en el puerto 80 con el siguiente link : https://[[HOST_SUBDOMAIN]]-80-[[KATACODA_HOST]].environments.katacoda.com/  

x

