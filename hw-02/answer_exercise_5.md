# Answer 5

**Diseña una estrategia de despliegue que se base en ”Blue Green”. Podéis utilizar la imagen del ejercicio 1**

_Respuesta_

1. Se tiene el deployment con la version 1 del cambio (Blue)

`kubectl apply -f deployment.yml`

2. Se crea un nuevo deployment con la version 2 del cambio (Green) 

`kubectl apply -f deployment2.yml`

3. Se realizan las pruebas de usuario

4. Se redirige el trafico del service hacia deployment2 subiendo la version en el yml

![serviceUpdateYml](http://shorturl.at/puvxF)