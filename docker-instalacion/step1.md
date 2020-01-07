Siga los siguientes pasos para instalar docker  

1. Actualice el indice de paquetes de `apt`    
`sudo apt-get update`{{execute}}  

2. Habilitar a apt para hacer uso de repositorios sobre HTTPS  
`sudo apt-get install apt-transport-https ca-certificates curl 
gnupg-agent software-properties-common`{{execute}}  

3.  Agregar la llave PGP oficial de Docker  
`curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -`{{execute}}  

4. Instale el repositorio estable  
`sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"`{{execute}}  

5. Actualice el indice de paquetes de `apt`  
`sudo apt-get update`{{execute}}  

6. Instale la última versión de  Docker CE y containerd.  
`sudo apt-get install docker-ce=18.06.1~ce~3-0~ubuntu`{{execute}}

7. Revise la versión de docker que ha sido instalada.  
`docker --version`{{execute}}