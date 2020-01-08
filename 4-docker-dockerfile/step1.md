
1. Clone el reopsitorio
`git clone https://github.com/reysillo/dockerfile.git`{{execute}}  


2. Ingrese a la carpeta demo  
`cd dockerfile`{{execute}}  

3. Revisión del contenidos  
`ls`{{execute}}    
`cat Dockerfile`{{execute}}  

4. Construcción  de la imagen  
`docker build -t mi-apache:1.0 .`{{execute}}  

5. Ejecución del contenedor  
`docker run -d  -p 80:80 mi-apache:1.0`{{execute}}  

6. Una vez ejecutado el contenedor se puede ver el resultado en el puerto 80 con el siguiente link : https://[[HOST_SUBDOMAIN]]-80-[[KATACODA_HOST]].environments.katacoda.com/  


d

