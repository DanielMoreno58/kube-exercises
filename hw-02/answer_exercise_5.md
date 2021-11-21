# Answer 5

**Diseña una estrategia de despliegue que se base en ”Blue Green”. Podéis utilizar la imagen del ejercicio 1**

_Respuesta_

1. Se crea un nuevo deployment con la version 2 del cambio (Green) 

`kubectl apply -f deployment2.yml`

2. Se realizan las pruebas de usuario

3. Se redirige el trafico del service hacia deployment2
