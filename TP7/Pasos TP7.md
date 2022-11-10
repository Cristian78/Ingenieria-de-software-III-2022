Ing. de Soft. III
TP7

Ejercicio 1

<img src="Imagenes TP7/1.1.jpg">

<img src="Imagenes TP7/1.2.jpg">

Ejercicio 2

Jenkins Pipeline es un conjunto de complementos que adminte la implementacion e integracion de canalizaciones de entrega continua. Podemos gestionar y administrar herramientas para crear jobs o pipelines que automaticen el proceso de despliegue de software.
El codigo de pipeline define todo el proceso de creacion, que normalmente incluye etapas para crear una aplicacion, probarla y luego entregarla.


Ejercicio 3

<img src="Imagenes TP7/1.3.jpg">

<img src="Imagenes TP7/1.4.jpg">


Ejercicio 4

<img src="Imagenes TP7/4.1.jpg">

<img src="Imagenes TP7/4.2.jpg">

<img src="Imagenes TP7/4.3.jpg">

Como vemos en el output se puede apreciar como recorre linea por linea el script hasta dar en la salida un "hello world" y se termina en SUCCESS


Ejercicio 5

<img src="Imagenes TP7/5.1.jpg">

<img src="Imagenes TP7/5.2.jpg">

En este caso en la primer imagen podemos ver que el script utiliza maven M3 y consta de stage y un post. Estos steps nos permite obtener un proyecto con mvn desde github y compilarlo, luego, se guarda los logs en un archivo y el ejectable .jar en una carpeta target


Ejercicio 6

Siguiendo el ejercicio 5 haremos los mismos pasos pero con la diferencia en el que modificaremos la direccion del repositorio por uno que se creo nuevo con el spring-boot del tp6

<img src="Imagenes TP7/6.1.jpg">

<img src="Imagenes TP7/6.2.jpg">


Ejercicio 7

//adjunto jenkinsfile_2