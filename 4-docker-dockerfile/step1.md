
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

Render port 80: https://[[HOST_SUBDOMAIN]]-80-[[KATACODA_HOST]].environments.katacoda.com/