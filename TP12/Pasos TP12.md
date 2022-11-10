Ing. de Soft. III
TP12

Ejercicio 1

Creamos la cuenta

<img src="Imagenes TP12/1.1.jpg">

<img src="Imagenes TP12/1.2.jpg">

Y luego iniciaremos sesion desde el CLI 

<img src="Imagenes TP12/1.3.jpg">

<img src="Imagenes TP12/1.4.jpg">


Ejercicio 2

Una vez que modificamos nuestro archivo de Dockerfile del spring-boot (los cambios estaran en su respectivo repo) continuaremos creando la app

<img src="Imagenes TP12/2.1.jpg">

Creado la app veremos que nos devuelve el nombre y la pagina la cual en mi caso es vast-eyrie-43305 donde estara la app

Lo siguiente sera generar y subir la imagen de docker al registry de Heroku desde donde este registry se desplegara la aplicacion en Heroku

<img src="Imagenes TP12/2.2.jpg">

Una vez terminado, se desplegara la aplicacion

<img src="Imagenes TP12/2.3.jpg">

Ahora podremos acceder a la aplicacion desde https://vast-eyrie-43305.herokuapp.com/

<img src="Imagenes TP12/2.4.jpg">