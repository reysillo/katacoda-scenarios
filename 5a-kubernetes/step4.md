## Desplegando un servicio público
`clear`{{execute}}  

1. Ver la lista de los deployments
`kube get deployments`{{execute}} 


2. En Kubernetes tambien se pueden desplegar varios recursos por medio de un yaml, por ejemplo lanzar un nginx con un balanceador de carga:  
`cat balancer_and_nginx.yaml`{{execute}} 

3. Ver la lista de los deployments para comprobar el deployment creado 
`kube get deployments`{{execute}} 

3. Ver la lista de los deployments para comprobar el servicio creado 
`kube get services`{{execute}} 


4. Como el nuevo servicio es de tipo load balancer kubernetes se comunicará con AWS para la creación pública del servicio
`kube describe deployment nginx-deployment`{{execute}} 