Ing. de Soft. III
TP8

Ejercicio 1
-Listar los pros y contras de este tipo de herramientas
-Sacar conclusiones

Una de las ventajas que podemos sacar con este tipo de herramientas es la velocidad que nos ofreceria pero eso tambien hace que aumente la complejidad de uso. La integracion continua nativa en la nuve necesita una mayor automatizacion y estabilidad y herramientas diseñadas para admitir la complejidad que surge del desarrollo en un entorno de microservicios


Ejercicio 2
    Configurando Github Actions

Desde github, trabajaremos desde el repositorio donde se encuentra la aplicacion de spring-boot, a partir de alli crearemos un workflow a partir del script que nos provee, ingresaremos a la opcion de action de github y modificaremos los parametros de la direccion para que tome nuestra aplicacion

<img src="Imagenes TP8/1.1.jpg">

<img src="Imagenes TP8/1.2.jpg">

Una vez modificado le daremos commit y luego iremos a la opcion de CI y lo correremos manualmente

<img src="Imagenes TP8/1.3.jpg">

<img src="Imagenes TP8/1.4.jpg">


Ejercicio 3

Guiandonos de la guia del tp7 y del punto anterior, empezamos creando un nuevo workflow, con el nombre docker-publish.yml
En ese mismo lugar modificaremos el script para que tome nuestros valores para el usuario y contraseña oculto de docker hub

<img src="Imagenes TP8/3.1.jpg">

En el apartado settings de github nos vamos a secrets y actions para generar los secreto

<img src="Imagenes TP8/3.2.jpg">

Lo corremos manualmente

<img src="Imagenes TP8/3.3.jpg">

Y verificaremos que se haya subido en docker hub

<img src="Imagenes TP8/3.4.jpg">

Ejercicio 4

Nos logueamos a CircleCI con github seleccionaremos la opciones y lo corremos

<img src="Imagenes TP8/4.1.jpg">

<img src="Imagenes TP8/4.2.jpg">