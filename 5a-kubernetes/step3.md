1. Desplegar un deployment desde la linea de comandos 
`k run nginx-deployment --image=nginx:1.16 --replicas=1`{{execute}} 

2. Ver la lista de los deployments
`k get deployments`{{execute}} 

3. Ver el detalle del nuevo deployment
`k describe nginx-deployment`{{execute}} 

4. Escalar un Deployment
`k scale deployment nginx-deployment --replicas=4`{{execute}} 

5. Ver la lista de los replicaset de un deployment
`k get rs`{{execute}} 

6. Ver la lista de los pods
`k get pods`{{execute}} 

7. Eliminar un deployment 
 `k delete deployment nginx-deployment `{{execute}}  