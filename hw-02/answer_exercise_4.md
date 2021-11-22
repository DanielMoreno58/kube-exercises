# Answer 4

Crear un objeto de tipo deployment con las especificaciones del ejercicio 1.

----

**1. Despliega una nueva versión de tu nuevo servicio mediante la técnica “recreate”**

_Respuesta_

Se uso el siguiente comando:

`kubectl apply -f deployment.yml`

![deployment](https://raw.githubusercontent.com/DanielMoreno58/kube-exercises/master/images/deployment.png)

----

**2. Despliega una nueva versión haciendo “rollout deployment”**

_Respuesta_

Se uso el siguiente comando:

`kubectl set image deployment.v1.apps/nginx-deployment nginx=nginx:1.19.5 --record=true`

![rolloutDeployment](https://raw.githubusercontent.com/DanielMoreno58/kube-exercises/master/images/rolloutDeployment.png)

![deploymentDescribe](https://raw.githubusercontent.com/DanielMoreno58/kube-exercises/master/images/describeDeployment.png)

----

**3. Realiza un rollback a la versión generada previamente**

_Respuesta_

Se usa el siguiente comando:

`kubectl rollout undo deployment nginx-deployment --to-revision=1`

![rolloutPreviousVersion](https://raw.githubusercontent.com/DanielMoreno58/kube-exercises/master/images/rolloutPreviousVersion.png)

