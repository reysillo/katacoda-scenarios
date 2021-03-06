`clear`{{execute}}  

1. Ver la lista de los deployments
`kube get deployments`{{execute}} 


2. En Kubernetes tambien se pueden desplegar recursos desde la linea de comandos, por ejemplo para desplegar un deployment de nginx:  
`kube run nginx-deployment --image=nginx:1.16 --replicas=1`{{execute}} 

3. Ver la lista de los deployments para comprobar el deployment creado 
`kube get deployments`{{execute}} 

4. Ver el detalle del nuevo deployment
`kube describe deployment nginx-deployment`{{execute}} 

5. Obtener la lista de los pods del namespace
`kube get pods`{{execute}}   

6. Escalar un Deployment
`kube scale deployment nginx-deployment --replicas=10`{{execute}} 

7. Ver la lista de los replicaset de un deployment
`kube get rs`{{execute}} 

8. Obtener la lista de los pods del namespace
`kube get pods`{{execute}}   

---
## Actualizando un Deployment  
`clear`{{execute}}  

1. Ver el detalle del nuevo deployment  
`kube describe deployment nginx-deployment`{{execute}} 

2. Actualizar un deployment
`kube set image deployment nginx-deployment nginx-deployment=nginx:1.17 --all`{{execute}} 

3. Ver la lista de los pods
`kube get pods`{{execute}} 

4. Actualizar el deployment a la versión xxx para generar un error
`kube set image deployment nginx-deployment nginx-deployment=nginx:xxx --all`{{execute}} 

5. Ver el estado de la actualización  
`kube rollout status deployment/nginx-deployment`{{execute}} 

5. Roll Back 
`kube rollout undo deployment/nginx-deployment`{execute}} 

6. Ver el deployment para validar el rollback 
`kube describe deployment nginx-deployment`{{execute}} 

7. Tambien podemos hacerlo modificando el yaml generado 
`kube set edit deployment nginx-deployment`{{execute}} 

8. Eliminar un deployment 
`kube delete deployment nginx-deployment `{{execute}}  