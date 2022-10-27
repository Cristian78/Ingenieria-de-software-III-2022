Ing. de Soft. III
TP3

1)
Creacion de red en docker

<img src= "Imagenes TP3/1.1.jpg">

Instanciar una base de datos Redis conectada a esa Red.

<img src= "Imagenes TP3/1.2.jpg">

Levantar una aplicacion web, que utilice esta base de datos

<img src= "Imagenes TP3/1.3.jpg">

Abrir un navegador y acceder a la URL: http://localhost:5000/

<img src= "Imagenes TP3/1.4.jpg">

<img src= "Imagenes TP3/1.5.jpg">

2)
Explicar cómo funciona el sistema:
	Es una API conectada a una base de datos Redis en el que tiene un contador la cual se va incrementando por cada visita

¿Para qué se sirven y porque están los parámetros -e en el segundo Docker run del ejercicio 1?
	Sirven para definir variables de entorno y estan en el ejercicio 1 para configurar el host y el puerto de Redis

¿Qué pasa si ejecuta docker rm -f web y vuelve a correr docker run -d --net mybridge -e REDIS_HOST=db -e REDIS_PORT=6379 -p 5000:5000 --name web alexisfr/flask-app:latest?
	Si ejecuto docker rm -f web y luego el siguiente comando, se eliminaria el contenedor y al levantarlo no se reiniciaria el contador ya que solo se elimino la aplicacion web

¿Qué occure en la página web cuando borro el contenedor de Redis con docker rm -f db?
	Al borrarlo no nos cargaria la pagina y ahi se borraria los registros de datos en este caso el contador

Y si lo levanto nuevamente con docker run -d --net mybridge --name db redis:alpine?
	Volveria a iniciar de nuevo la pagina como en su principio

¿Qué considera usted que haría falta para no perder la cuenta de las visitas?
	Crear con docker otro contenedor de datos para guardar informacion sin importar el contenedor

(Se eliminaron los elementos creados)


3)
Se creo el archivo docker-compose.yml y se ejecuto

<img src= "Imagenes TP3/3.1.jpg">

<img src= "Imagenes TP3/3.2.jpg">

Al realizar la ejecucion, el docker compose lo que hizo fue realizar todo el ejercicio del punto 1 pero de forma automatica con solo crear un script en el archivo .yml


4)
<img src= "Imagenes TP3/4.1.jpg">

<img src= "Imagenes TP3/4.2.jpg">

Explicar como está configurado el sistema, puertos, volumenes componenetes involucrados, utilizar el Docker compose como guía.

En la configuracion del sistema tiene 5 servicios que son:
	1- vote: Es una aplicacion que nos permite emitir el voto
	2- result: Aplicacion que nos permite visualizar el resultado de la votacion
	3- worker: Es el que recibe los votos y los manda a la base de datos
	4- redis: Una cola que recolecta los votos
	5- db: Base de datos que almacena los votos

Tiene los puertos al host 5000:80, 5001:80, 5858:5858