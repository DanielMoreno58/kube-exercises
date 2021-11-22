# Answer 3

**Creación de Service**

Crear un objeto de tipo service para exponer la aplicación del ejercicio anterior de las siguientes formas:

----

**Exposicion de servicios kubernetes** 

![exposeServices](https://raw.githubusercontent.com/DanielMoreno58/kube-exercises/master/images/exposeServices.png)

----

**1. Exponiendo el servicio hacia el exterior (crea service1.yaml)**

_Respuesta_

Se genera un nuevo servicio con el siguiente comando:

`kubectl create -f service1.yml`

----

**2. De forma interna, sin acceso desde el exterior (crea service2.yaml)**

_Respuesta_

Se genera un nuevo servicio con el siguiente comando:

`kubectl create -f service2.yml`


----

**3. Abriendo un puerto especifico de la VM (crea service3.yaml)**

_Respuesta_

Se genera un nuevo servicio con el siguiente comando:

`kubectl create -f service3.yml`

