Ing. de Soft. III
TP9

Ejercicio 1

Dependencia: En el archivo pom.xml del proyecto spring-boot, existe la dependencia de spring-boot-starter-test, que es un starter para realizar testeos de las aplcaciones de spring-boot, esta las realiza con Junit, Hamcrest y Mockito

Analizando el metodo HelloWorldServiceTest tenemos @Test, este pertenece a Junit que identifica un metodo como metodo de prueba. Luego la instancia HelloWorldServiceTest que mediante una declaracion assertEquials verifica si el mensaje ingresado a traves del metodo getHelloMessage() sea igual o retorne el mensaje "Spring boot says hellos from a Docker container"

<img src="Imagenes TP9/1.1.jpg">


Ejercicio 3

Analizando el test ExampleInfoContributorTest se puede ver que crea un objeto mock de la clase Info.Builder.class que tiene el nombre builder, luego, el metodo contribute trae informacion de la clase ExampleInfoContributor y luego verifica que la clase contenga algun tipo de dato

<img src="Imagenes TP9/1.2.jpg">


Ejercicio 4

Primero agregaremos el unit test a la clase HelloWorldServiceTest para el retorno de hola hola y hello hello

<img src="Imagenes TP9/4.1.jpg">

Se crearan las clases AbrstractTest y SampleControllerTest

Luego lo correremos y el test se ejecuta correctamente

<img src="Imagenes TP9/4.2.jpg">


Ejercicio 6

Para este ejercicio se utilizo github y creamos un workflow llamado maven.yml

<img src="Imagenes TP9/6.2.jpg">

<img src="Imagenes TP9/6.1.jpg">