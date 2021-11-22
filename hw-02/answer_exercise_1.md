# Answer 1

**1. ¿Cómo puedo obtener las últimas 10 líneas de la salida estándar (logs generados por la aplicación)?**

_Respuesta_

Usaria el siguiente comando:

`kubectl logs -f --tail 10 nginx`

![getLast10Logs](https://raw.githubusercontent.com/DanielMoreno58/kube-exercises/master/images/getLast10Logs.png)

-----

**2. ¿Cómo podría obtener la IP interna del pod? Aporta capturas para indicar el proceso que seguirías.**

_Respuesta_

Usaria el siguiente comando que muestra toda la información del pod:

`kubectl describe pods nginx`

![getIPPod](https://raw.githubusercontent.com/DanielMoreno58/kube-exercises/master/images/getIpPods.png)

-----

**3. ¿Qué comando utilizarías para entrar dentro del pod?**

_Respuesta_

Usaria el siguiente comando:

`kubectl exec --stdin --tty nginx  -- /bin/bash`


![getInsidePod](https://raw.githubusercontent.com/DanielMoreno58/kube-exercises/master/images/getInsidePod.png)

-----

**4. ¿Necesitas visualizar el contenido que expone NGINX, ¿qué acciones debes llevar a cabo?**

_Respuesta_

Usaria el siguiente comando:

`kubectl port-forward nginx 8080:80`

![getPortForward](https://raw.githubusercontent.com/DanielMoreno58/kube-exercises/master/images/portForward.png)

![getPortForwardChrome](https://raw.githubusercontent.com/DanielMoreno58/kube-exercises/master/images/portForwardChrome.png)


-----

**5. Indica la calidad de servicio (QoS) establecida en el pod que acabas de crear. ¿Qué lo has mirado?**

_Respuesta_

Lo vemos con el siguiente comando:

`kubectl describe pods nginx`

![getQuosClass](https://raw.githubusercontent.com/DanielMoreno58/kube-exercises/master/images/getQuosClass.png)

Un pod con una clase Guaranteed debe tener lo siguiente:

* Todo contenedor debe tener una memoria límite
* Todo contenedor debe tener un límite de CPU

Esto se lo hemos indicado nosotros al momento de crear el pod en el yml como se muestra a continuacion:

![getLimits](https://raw.githubusercontent.com/DanielMoreno58/kube-exercises/master/images/getLimits.png)