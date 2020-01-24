1. Desplegar un deployment desde la linea de comandos 
`kube run nginx-deployment --image=nginx:1.16 --replicas=1`{{execute}} 

2. Ver la lista de los deployments
`kube get deployments`{{execute}} 

3. Ver el detalle del nuevo deployment
`kube describe nginx-deployment`{{execute}} 

4. Escalar un Deployment
`kube scale deployment nginx-deployment --replicas=10`{{execute}} 

5. Ver la lista de los replicaset de un deployment
`kube get rs`{{execute}} 

6. Ver la lista de los pods
`kube get pods`{{execute}} 

7. Actualizar un deployment
`kube set image deployment nginx-deployment nginx=nginx:1.17 --all`{{execute}} 

8. Ver la lista de los replicaset de un deployment
`kube get rs`{{execute}} 

9. Ver la lista de los pods
`kube get pods`{{execute}} 

10. Tambien podemos hacerlo modificando el yaml generado 
`kube set edit deployment nginx-deployment`{{execute}} 

11. Eliminar un deployment 
`kube delete deployment nginx-deployment `{{execute}}  