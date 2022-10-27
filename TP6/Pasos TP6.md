Ing. de Soft. III
TP6

Ejercicio 1
    Describir las instrucciones

    FROM: La instrucción FROM especifica la imagen principal a partir de la cual se está construyendo 
    
    RUN: El comando docker run crea y arranca un contenedor para ejecutar unos comandos ya establecidos en el Dockerfile o los que se pasen como un parámetro.
    
    COPY y ADD: son instrucciones de Dockerfile que tienen propósitos similares. Le permiten copiar archivos desde una ubicación específica en una imagen de Docker. COPY toma src y destrucción. Solo le permite copiar en un directorio local o desde su host (la máquina que crea la imagen de Docker) en la propia imagen de Docker. ADD también  te permite hacer eso, pero también admite otras 2 fuentes. Primero, puede usar una URL en lugar de un archivo / directorio local. En segundo lugar, puede extraer tar del directorio de origen al destino.
    
    EXPOSE: La instrucción EXPOSE expone un puerto en particular con un protocolo específico dentro de un contenedor Docker. En el término más simple, la instrucción EXPOSE le dice a Docker que obtenga toda la información requerida durante el tiempo de ejecución de un puerto específico. Estos puertos pueden ser TCP o UDP, pero es TCP de forma predeterminada.
    
    CMD: Este comando se encarga de pasar valores por defecto a un contenedor. Entre estos valores se pueden pasar ejecutables.
    
    ENTRYPOINT: Este comando se ejecuta cuando se quiere ejecutar un ejecutable en el contenedor en su arranque. Los ejemplos tipo de su uso, son cuando se quiere levantar un servidor web, una base de datos, etc

Ejercicio 2
    Compilar la salida

<img src="Imagenes TP6/2.1.jpg">

-Agregar un archivo llamado Dockerfile (en el directorio donde se corrió el comando mvn)

<img src="Imagenes TP6/2.2.jpg">

-Generar la imagen de docker con el comando build

<img src="Imagenes TP6/2.3.jpg">

-Ejecutar el contenedor

<img src="Imagenes TP6/2.4.jpg">

-Verificar si retorna un mensaje (correr en otro terminal o browser)

<img src="Imagenes TP6/2.5.jpg">


Ejercicio 3

-Construir nuevamente la imagen con la modificacion del dockerfile

<img src="Imagenes TP6/3.1.jpg">

Al realizar el cambio en el contenido del dockerfile lo que sucede es que genera una nueva secuencia de instrucciones que compila el codigo y genera los archivos .jar para su ejecucion, luego, en vez de partir en una imagen maven, parte de una imagen de java lo que hace que se reduzca su tamaño, copia el archivo .jar anterior y lo ejecuta, generando una imagen similar al punto anterior.


Ejercicio 4

<img src="Imagenes TP6/4.1.jpg">

-Explicar que sucedio

Se levantaron 2 contenedores, uno app y otro redis, en el que, el contenedor app se creo a partir de una imagen que a su vez se creo a partir del archivo de dockerfile encontrado en la raiz del directorio del proyecto
Docker-compose permite esto mediante la especificacion de la ubicacion de dicho archivo mediante la key build.context


Ejercicio 5

docker build -f Dockerfile.dockerfile -t test-node

docker run -p 3000:80 test-node

Ejercicio 6

<img src="Imagenes TP6/6.1.jpg">