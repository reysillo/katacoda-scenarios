Los comandos más comunes para el trabajo con pods en Kubernetes son:

  * 'kubectl get': lista los recursos 
  * 'kubectl describe': muestra información detallada sobre un recurso 
  * 'kubectl logs': imprime los logs de un contenedor en una vaina 
  * 'kubectl exec': ejecuta un comando en un contenedor de un pod  

`clear`{{execute}}  

1. Crear un alias con el comando kubectl y el namespace creado anteriormente
`alias kube='kubectl -n []'`

2. Obtener la lista de los pods del namespace
`kube get pods`{{execute}}    

3. En kubernetes se pueden crear nuevos recursos por medio de un archivo .yaml por ejemplo para crear un pod se usaría el siguiente archvio:  
`cat pod.yaml`{{execute}}  

4. Para crear los recursos se utiliza el comando apply  
`kube apply -f pod.yaml`{{execute}}  

5. Obtener la lista de los pods del namespace para verificar la creación del pod 
`kube get pods`{{execute}}    

6. Ver los detalles del nuevo pod creado  
`kube describe pod []`  

7. Ver los logs del nuevo pod creado  
`kube logs []`

8. Ejecutar un comando dentro de un contenedor  
`kube exec [] ls`  

9. Eliminar un pod  
`kube delete pod []`  

10. Eliminar recursos desde un archivo yaml  
`kube delete -f pod.yaml`{{execute}}  
