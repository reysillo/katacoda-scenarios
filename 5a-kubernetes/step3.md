`clear`{{execute}}  

1. Ver la lista de los deployments
`kube get deployments`{{execute}} 


2. En Kubernetes tambien se pueden desplegar recursos desde la linea de comandos, por ejemplo para desplegar un deployment de nginx:  
`kube run nginx-deployment --image=nginx:1.16 --replicas=1`{{execute}} 

3. Ver la lista de los deployments para comprobar el deployment creado 
`kube get deployments`{{execute}} 

3. Ver el detalle del nuevo deployment
`kube describe deployment nginx-deployment`{{execute}} 

2. Obtener la lista de los pods del namespace
`kube get pods`{{execute}}   

4. Escalar un Deployment
`kube scale deployment nginx-deployment --replicas=10`{{execute}} 

5. Ver la lista de los replicaset de un deployment
`kube get rs`{{execute}} 

2. Obtener la lista de los pods del namespace
`kube get pods`{{execute}}   

4. Escalar un Deployment
`kube scale deployment nginx-deployment --replicas=2`{{execute}} 


6. Ver la lista de los pods
`kube get pods`{{execute}} 

---
`clear`{{execute}}  

7. Ver el detalle del nuevo deployment
`kube describe deployment nginx-deployment`{{execute}} 

8. Actualizar un deployment
`kube set image deployment nginx-deployment nginx-deployment=nginx:1.17 --all`{{execute}} 


9. Ver la lista de los pods
`kube get pods`{{execute}} 

10. Actualizar un deployment
`kube set image deployment nginx-deployment nginx-deployment=nginx:xxx --all`{{execute}} 

Roll Back 
`kubectl rollout undo deployments/nginx-deployment`
{execute}} 

11. Ver la lista de los replicaset de un deployment
`kube get rs`{{execute}} 

12. Ver la lista de los pods
`kube get pods`{{execute}} 

13. Tambien podemos hacerlo modificando el yaml generado 
`kube set edit deployment nginx-deployment`{{execute}} 

14. Eliminar un deployment 
`kube delete deployment nginx-deployment `{{execute}}  