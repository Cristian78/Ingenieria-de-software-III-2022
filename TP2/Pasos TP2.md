Ing. de Soft. III

1)Instalacion del docker

Ejecutar el siguiente comando para comprobar versiones de cliente y demonio.

<img src= "Imagenes TP2/1.jpg">

2)"Registro en docker"

3)Imagen obtenida y version

Bajar una imagen de DockerHub

<img src= "Imagenes TP2/3.1.jpg">

Verificar qué versión y tamaño tiene la imagen bajada, obtener una lista de imágenes locales

<img src= "Imagenes TP2/3.2.jpg">

4)Ejecucion de contenedores

Ejecutar un contenedor

<img src= "Imagenes TP2/4.1.jpg">

Explicar porque no se obtuvo ningún resultado
    
    No se obtuvo nada debido a que no se especifico que obtener en el comando

Especificamos algún comando a correr dentro del contendor

<img src= "Imagenes TP2/4.2.jpg">

Ver los contendores ejecutados

<img src= "Imagenes TP2/4.3.jpg">

Vemos que no existe nada en ejecución, correr entonces:
docker ps -a
Mostrar el resultado y explicar que se obtuvo como salida del comando anterior.

<img src= "Imagenes TP2/4.4.jpg">

    En este caso optenemos todos los contenedores por default que se esten corriendo.

5)Ejecucion modo interactivo

<img src= "Imagenes TP2/5.1.jpg

6)Borrando contenedores

Obtener la lista de contendores

<img src= "Imagenes TP2/6.1">

Para borrar podemos utilizar el id o el nombre (autogenerado si no se especifica) de contendor que se desee.

<img src= "Imagenes TP2/6.2">

Borrar todos los contendores que no estén corriendo.

<img src= "Imagenes TP2/6.3">

7) Montando volumenes

Hasta este punto los contenedores ejecutados no tenían contacto con el exterior, ellos corrían en su propio entorno hasta que terminaran su ejecución. Ahora veremos cómo montar un volumen dentro del contenedor para visualizar por ejemplo archivos del sistema huésped:

<img src= "Imagenes TP2/7.1">

<img src= "Imagenes TP2/7.2">

Verificar que el Archivo se ha creado en el escritorio o en el directorio home según corresponda.

<img src= "Imagenes TP2/7.3">

8)Publicando puertos

En el caso de aplicaciones web o base de datos donde se interactúa con estas aplicaciones a través de un puerto al cual hay que acceder, estos puertos están visibles solo dentro del contenedor. Si queremos acceder desde el exterior deberemos exponerlos.

<img src= "Imagenes TP2/8.1">

<img src= "Imagenes TP2/8.2">

<img src= "Imagenes TP2/8.3">

Ahora pudimos acceder al contenedor desde el localhost

9)Base de datos

Levantar una base de datos PostgreSQL

<img src= "Imagenes TP2/9.1">

Ejecutar sentencias utilizando esta instancia

<img src= "Imagenes TP2/9.2">

<img src= "Imagenes TP2/9.3">

<img src= "Imagenes TP2/9.4">

<img src= "Imagenes TP2/9.5">
