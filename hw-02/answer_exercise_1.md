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


-----

**5. Indica la calidad de servicio (QoS) establecida en el pod que acabas de crear. ¿Qué lo has mirado?**

_Respuesta_