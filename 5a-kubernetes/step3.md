1. Desplegar un deployment desde la linea de comandos 
`k run nginx-deployment --image=nginx:1.16 --replicas=1`{{execute}} 

2. Ver la lista de los deployments
`k get deployments`{{execute}} 

3. Ver el detalle del nuevo deployment
`k describe nginx-deployment`{{execute}} 

4. Escalar un Deployment
`k scale deployment nginx-deployment --replicas=10`{{execute}} 

5. Ver la lista de los replicaset de un deployment
`k get rs`{{execute}} 

6. Ver la lista de los pods
`k get pods`{{execute}} 

7. Actualizar un deployment
`k set image deployment nginx-deployment nginx=nginx:1.17 --all`{{execute}} 

5. Ver la lista de los replicaset de un deployment
`k get rs`{{execute}} 

6. Ver la lista de los pods
`k get pods`{{execute}} 

8. Tambien podemos hacerlo modificando el yaml generado 
`k set edit deployment nginx-deployment`{{execute}} 

9. Eliminar un deployment 
 `k delete deployment nginx-deployment `{{execute}}  