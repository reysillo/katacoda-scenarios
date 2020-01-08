## Montar un archivo o carpeta local a un contenedor

1. Crear una carpeta en local  
`mkdir mi-carpeta-local`{{execute}}  
`ls mi-carpeta-local`{{execute}}  

2. Crear un nuevo archivo local  
 `touch mi-carpeta-local/mi-archivo1.txt`{{execute}}  
 `ls mi-carpeta-local`{{execute}}  

3. Iniciar un contenedor con un volumen a partir de mi-carpeta-local  
. `docker run -it --name contenedor2 -v $(pwd)/mi-carpeta-local:carpeta-en-docker ubuntu`{{execute}} 

4. Verificación del  la carpeta montada dentro del contenedor    
`ls /carpeta-en-docker`{{execute}}  

5. Crear un nuevo archivo en el contenedor  
 `touch /carpeta-en-docker/mi-archivo2.txt`{{execute}}  

6. Salir del contenedor  
`exit`{{execute}}  

7. Verificación del contenido de la carpeta local  
`ls mi-carpeta-local`{{execute}}  

Identifique que el archivo mi-archivo2.txt ha sido creado dentro del docker en la carpeta local  