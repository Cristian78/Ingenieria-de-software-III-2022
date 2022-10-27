Ing. de Soft. III
TP4

1)

<img src= "Imagenes TP4/1.1.jpg">

<img src= "Imagenes TP4/1.2.jpg">

<img src= "Imagenes TP4/1.3.jpg">

<img src= "Imagenes TP4/1.4.jpg">

2)

Pregunta 1
    Describa los contenedores creados, indicando cuales son los puntos de ingreso del sistema

    [Puerto 80 | Enpoint /app] docker-compose-catalogue-1
    [Puerto 80 | Endpoint /user] docker-compose-user-1
    [Puerto 27017] docker-compose-carts-db-1
    [] docker-compose-carts-1
    [Puerto 3306] docker-compose-catalogue-db-1
    [Puerto 27017] docker-compose-orders-db-1
    [puerto 8079] docker-compose-front-end-1
    [] docker-compose-queue-master-1
    [Puertos 4369 / 5671-5672 / 25672] docker-compose-rabbitmq-1
    [Puerto 80] docker-compose-payment-1
    [] docker-compose-orders-1
    [] docker-compose-shipping-1
    [Puerto 27017] docker-compose-user-db-1
    [Puertos 80 / 8080] docker-compose-edge-router-1

Pregunta 2
<img src= "Imagenes TP4/2.jpg">

Pregunta 3
    ¿Por qué cree usted que se está utilizando repositorios separados para el código y/o la configuración del sistema? Explique puntos a favor y en contra.

    Se utilizan repositorios separados porque cada contenedor es un proyecto separado en el que cada uno nos brindara un servicio. Un punto a favor es el hecho de que se puede trabajar de forma independiente en cada uno de los microservicios. Un punto en contra que podria destacar es el mismo hecho de tener separado hace que la cantidad de repositorios aumentara y en el caso de que sean mucho pueden llegar a generar problemas de organizacion

Pregunta 4
    ¿Cuál contenedor hace las veces de API Gateway?
    
    El contenedor es el de edge-router

Pregunta 5
<img src= "Imagenes TP4/2.5.jpg">

Pregunta 6
    ¿Cuál de todos los servicios está procesando la operación?

    El que esta procesando la operacion es el frontend que deriva a customer

Pregunta 7
    ¿Y para los siguientes casos?

    En estos casos el frontend deriva la requests a catalogue
<img src= "Imagenes TP4/2.7.jpg">

Pregunta 8
    ¿Como persisten los datos los servicios?
    
    Los datos persisten en cada contenedor en las que contiene el nombre "db"

Pregunta 9
    ¿Cuál es el componente encargado del procesamiento de la cola de mensajes?

    El componente encargado es queue-master-1

Pregunta 10
    ¿Qué tipo de interfaz utilizan estos microservicios para comunicarse?

    Utilizan API rest