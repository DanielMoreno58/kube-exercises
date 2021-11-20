# Answer 2

**Explicacion**

Crear un objeto de tipo replicaSet a partir del objeto anterior

_Respuesta_

Se crea un Replica Set agregando un nuevo fichero llamado **_replicaset.yml_** donde se indica las tres replicas de un pod en base a una imagen nginx, para ello se usa el siguiente comando:

`kubectl create -f replicaset.yml`

![createReplicaSet](http://shorturl.at/asKNV)

**1. ¿Cúal sería el comando que utilizarías para escalar el número de replicas a 10?**

**2. Si necesito tener una replica en cada uno de los nodos de Kubernetes, ¿qué objeto se adaptaría mejor?**