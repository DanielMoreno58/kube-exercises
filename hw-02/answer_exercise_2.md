# Answer 2

**Creación de ReplicaSet**

Crear un objeto de tipo replicaSet a partir del objeto anterior

_Respuesta_

Se crea un Replica Set agregando un nuevo fichero llamado **_replicaset.yml_** donde se indica las tres replicas de un pod en base a una imagen nginx, para ello se usa el siguiente comando:

`kubectl create -f replicaset.yml`

![createReplicaSet](https://raw.githubusercontent.com/DanielMoreno58/kube-exercises/master/images/createReplicaSet.png)

----

**1. ¿Cúal sería el comando que utilizarías para escalar el número de replicas a 10?**

_Respuesta_

Con el siguiente comando:

`kubectl scale --replicas=10 rs/nginx-replica`

![scaleReplicaset](https://raw.githubusercontent.com/DanielMoreno58/kube-exercises/master/images/scaleReplicaset.png)

----

**2. Si necesito tener una replica en cada uno de los nodos de Kubernetes, ¿qué objeto se adaptaría mejor?**

_Respuesta_

DaemonSet