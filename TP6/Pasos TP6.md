Ing. de Soft. III
TP6

Ejercicio 1)
Describir las instrucciones

    FROM: La instrucción FROM especifica la imagen principal a partir de la cual se está construyendo 
    
    RUN: El comando docker run crea y arranca un contenedor para ejecutar unos comandos ya establecidos en el Dockerfile o los que se pasen como un parámetro.
    
    COPY y ADD: son instrucciones de Dockerfile que tienen propósitos similares. Le permiten copiar archivos desde una ubicación específica en una imagen de Docker. COPY toma src y destrucción. Solo le permite copiar en un directorio local o desde su host (la máquina que crea la imagen de Docker) en la propia imagen de Docker. ADD también  te permite hacer eso, pero también admite otras 2 fuentes. Primero, puede usar una URL en lugar de un archivo / directorio local. En segundo lugar, puede extraer tar del directorio de origen al destino.
    
    EXPOSE: La instrucción EXPOSE expone un puerto en particular con un protocolo específico dentro de un contenedor Docker. En el término más simple, la instrucción EXPOSE le dice a Docker que obtenga toda la información requerida durante el tiempo de ejecución de un puerto específico. Estos puertos pueden ser TCP o UDP, pero es TCP de forma predeterminada.
    
    CMD: Este comando se encarga de pasar valores por defecto a un contenedor. Entre estos valores se pueden pasar ejecutables.
    
    ENTRYPOINT: Este comando se ejecuta cuando se quiere ejecutar un ejecutable en el contenedor en su arranque. Los ejemplos tipo de su uso, son cuando se quiere levantar un servidor web, una base de datos, etc

    