## Crear un volumen al vuelo 
Kubernetes tiene su herramienta de linea de comandos llamada kubectl que necesita del archivo ~/.kube/config para poder comunicarse con el cluster de ek8s  

1. Revisión del archivo de cofiguración ~/.kube/config
`cat ~/.kube/config`{{execute}}  

2. Ver los detalles del cluster  
`kubectl cluster-info`{{execute}}    

3. Ver los nodos/servidores conectado al cluster  
`kubectl get nodes`{{execute}}  