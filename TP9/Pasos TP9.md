Ing. de Soft. III
TP9

Ejercicio 1

Dependencia: En el archivo pom.xml del proyecto spring-boot, existe la dependencia de spring-boot-starter-test, que es un starter para realizar testeos de las aplcaciones de spring-boot, esta las realiza con Junit, Hamcrest y Mockito

Analizando el metodo HelloWorldServiceTest tenemos @Test, este pertenece a Junit que identifica un metodo como metodo de prueba. Luego la instancia HelloWorldServiceTest que mediante una declaracion assertEquials verifica si el mensaje ingresado a traves del metodo getHelloMessage() sea igual o retorne el mensaje "Spring boot says hellos from a Docker container"