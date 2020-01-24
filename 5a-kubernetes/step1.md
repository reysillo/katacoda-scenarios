 Kubernetes tiene su herramienta de linea de comandos llamada kubectl que necesita del archivo ~/.kube/config para poder comunicarse con el cluster ek8s  

1. Revisión del archivo de cofiguración ~/.kube/config
`cat ~/.kube/config`{{execute}}  

2. Ver los detalles del cluster  
`kubectl cluster-info`{{execute}}    

3. Ver los nodos/servidores conectado al cluster (división física)
`kubectl get nodes`{{execute}}  

4. Ver los namespaces que componen el cluster
`kubectl get namespaces`{{execute}}  

5. Crear un namespace 
`kubectl create namespace []`

6. Confirmar la creación del namespace
`kubectl get namespaces`{{execute}}  

7. Ver los servicios de un namespace
`kubectl get services -n kube-system`{{execute}}  

8. Ver los servicios de todos los namespace
`kubectl get services --all-namespaces`{{execute}}  