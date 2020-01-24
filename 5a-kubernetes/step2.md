Los comandos más comunes para el trabajo con pods en Kubernetes son:

  * kubectl get - lista los recursos 
  * kubectl describe: muestra información detallada sobre un recurso 
  * kubectl logs: imprime los logs de un contenedor en una vaina 
  * kubectl exec: ejecuta un comando en un contenedor de un pod

1. Crear un alias con el comando kubectl y el namespace creado anteriormente
`alias k='kubectl -n []'`

2. Obtener la lista de los pods del namespace
`k get pods`{{execute}}    

3. Crear recursos desde un archivo yaml
`cat pod.yaml`{{execute}}  
`k apply -f pod.yaml`{{execute}}  

4. Ver los detalles del nuevo pod creado
`k describe pod []`

5. Ver los logs del nuevo pod creado
`k logs []`

6. Ejecutar un comando dentro de un contenedor
`k exec [] ls`

7. Eliminar un pod
`k delete pod []`

8. Eliminar recursos desde un archivo yaml
`k delete -f pod.yaml`{{execute}}  
