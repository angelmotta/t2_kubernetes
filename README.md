# Deploying kubernetes

## 1. Deploying Kubernetes single and multi-node

Para todos los casos que se van a mostrar a continuación se estará utilizando un deployment del cluster con el driver 'docker' donde cada nodo esta corriendo sobre un container tal como se mostrará en las siguiente secciones.
### 1.1 Creación de cluster Kubernetes local con un único nodo

* Creación de cluster

```
$ minikube start
```

<img src="images/minikube-start.png" width="65%">

* Podemos ver la información del cluster single-node y del con los comandos

```
$ kubectl cluster-info
$ kubectl get nodes -o wide
```

<img src="images/singlenode_cluster-info.png" width="65%">

* Adicionalmente podemos ver los PODs desplegados por defecto 

```
$ kubectl get pods -A
```

<img src="images/singlenode_get_pods.png" width="65%">

### 1.2 Creación de cluster Kubernetes local multi-nodo

* Para la creación del cluster multi-node especificamos un cluster de 2 nodos llamado 'multinode-demo' con el comando

```
minikube start --nodes 2 -p multinode-demo
```

<img src="images/minikube-start-cluster.png" width="65%">

* De forma similar podemos listar los nodos del cluster y apreciar los 2 nodos desplegados.

<img src="images/multinode_cluster-info.png" width="65%">

* En esta ocasión si listamos los PODs del cluster se puede ver como algunos de estos estan desplegados en el segundo nodo del cluster

<img src="images/multinode_get_pods.png" width="75%">

## 2. A Containerized application

## 3. Deployment a containerized application on Kubernetes
