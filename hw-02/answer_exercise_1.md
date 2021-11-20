# Answer 1

**1. ¿Cómo puedo obtener las últimas 10 líneas de la salida estándar (logs generados por la aplicación)?**

_Respuesta_

Usaria el siguiente comando:

`kubectl logs -f --tail 10 nginx`

![getLast10Logs](http://shorturl.at/erwLQ)

-----

**2. ¿Cómo podría obtener la IP interna del pod? Aporta capturas para indicar el proceso que seguirías.**

_Respuesta_

Usaria el siguiente comando que muestra toda la información del pod:

`kubectl describe pods nginx`

![getIPPod](http://shorturl.at/ijHL7)

-----

**3. ¿Qué comando utilizarías para entrar dentro del pod?**

_Respuesta_

Usaria el siguiente comando:

`kubectl exec --stdin --tty nginx  -- /bin/bash`


![getInsidePod](http://shorturl.at/jzRTY)

-----

**4. ¿Necesitas visualizar el contenido que expone NGINX, ¿qué acciones debes llevar a cabo?**

_Respuesta_

Usaria el siguiente comando:

`kubectl port-forward nginx 8080:80`

![getPortForward](http://shorturl.at/cBHJP)

![getPortForwardChrome](http://shorturl.at/glpER)


-----

**5. Indica la calidad de servicio (QoS) establecida en el pod que acabas de crear. ¿Qué lo has mirado?**

_Respuesta_

Lo vemos con el siguiente comando:

`kubectl describe pods nginx`

![getQuosClass](http://shorturl.at/nquHX)

Un pod con una clase Guaranteed debe tener lo siguiente:

* Todo contenedor debe tener una memoria límite
* Todo contenedor debe tener un límite de CPU

Esto se lo hemos indicado nosotros al momento de crear el pod en el yml como se muestra a continuacion:

![getLimits](http://shorturl.at/prIS1)