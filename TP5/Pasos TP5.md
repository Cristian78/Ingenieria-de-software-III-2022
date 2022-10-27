Ing. de Soft. III
TP5

1)
	Instalacion Java JDK y control de config
	
<img src= "Imagenes TP5/1.1.jpg">

2)
	Instalacion Maven

3)
Que es Maven?
	Es una herramienta de gestion de proyectos, simplifica procesos de build, sin la necesidad de proecuparse de los modulos, dependencias y librerias que necesite el proyecto

Que es el archivo POM?
	La unidad básica de trabajo en Maven es el llamado Modelo de Objetos de Proyecto conocido simplemente como POM (de sus siglas en inglés: Project Object Model).
	Se trata de un archivo XML llamado pom.xml que se encuentra por defecto en la raíz de los proyectos y que contiene toda la información del proyecto: su configuración y sus dependencias.
	
	-modelVersion: Define la version de Maven que utiliza el proyecto
	-groupId: Define el nombre de la libreria
	-artifactId: Define el nombre del proyecto, del target a generar
	-versionId: Define la version de la libreria que se esta desarrolando

Repositorios
	
	-Local: El repositorio local es un directorio en la computadora donde se ejecuta Maven. ALmacena en cache las descargas remotas y contiene artefactos de compilacion.
	-Central: Por defecto se buscan las dependencias que se necesiten en este repositorio, global y publico.
	-Remoto: Los repositorios remotos se refieren a cualquier otro tipo de repositorio, al que se accede mediante una variedad de protocolos file:// y https://. Estos repositorios puede ser un repositorio verdaderamente remoto configudaro por un tercero para proporcionar sus artefactos para descargar. Otros repositorios "remotos" pueden ser repositorios internos configurados en un servidor de archivos o HTTP dentro de su empresa, utilizados para compartir artefactos privados entre equipos de desarrollo y para lanzamientos.

Ciclo de vida

	-Default, que gestiona la construcción y despliegue del proyecto.
	-Clean, que gestiona la limpieza del directorio del proyecto. Es decir, se encarga de eliminar todos los archivos generados en el proceso de construcción y despliegue.
	-Site, que gestiona la creación de la documentación del proyecto.


Ejecutando mvn clean install

<img src= "Imagenes TP5/2.1.jpg">

Viendo los resultados en la carpeta se obtuvo un ejecutable .jar de un proyecto de otro repositorio

4)
	Maven continuacion

<img src= "Imagenes TP5/4.1.jpg">
<img src= "Imagenes TP5/4.2.jpg">

-Analizar la estructura de directorios generada
	A partir de la escructura de directorios generada se puede ver como se crean sub carpetas para cada elemento separados donde el ultimo es el ejecutable.

-Compilar el proyecto
-Analizar la salida del comando anterior y luego ejecutar el programa

<img src= "Imagenes TP5/4.3.jpg">


6)
	Manejo de dependiencias

-Crear un nuevo proyecto con artifactId ejemplo-uber-jar
-Modificar el código de App.java para agregar utilizar una librería de logging

<img src= "Imagenes TP5/6.2.jpg">

-Compilar el código e identificar el problema.

<img src= "Imagenes TP5/6.3.jpg">

	El error se debe a que en el pom.xml no se encuentra definido el logeo como dependencia, por ello, cuando se compila el maven no lo ejecuta

-Agregar la dependencia necesaria al pom.xml

<img src= "Imagenes TP5/6.4.jpg">

-Verificar si se genera el archivo jar y ejecutarlo

<img src= "Imagenes TP5/6.5.jpg">

<img src= "Imagenes TP5/6.6.jpg">


-Ahora, ejecutar la clase con el siguiente comando (en windows reemplazar $HOME por %USERPROFILE%, y separar por ; en lugar de :)

<img src= "Imagenes TP5/6.7.jpg">


-Implementar la opción de uber-jar: https://maven.apache.org/plugins/maven-shade-plugin/

<img src= "Imagenes TP5/6.8.jpg">

-Volver a generar la salida y probar ejecutando

<img src= "Imagenes TP5/6.9.jpg">


7)
	Importar desde Eclipse

<img src= "Imagenes TP5/7.1.jpg">

	Ejecucion

<img src= "Imagenes TP5/7.2.jpg">


8)

	Instalado Nodejs*
	Crear una nueva aplicacion

<img src= "Imagenes TP5/8.1.jpg">

	Ejecucion

<img src= "Imagenes TP5/8.2.jpg">


-Analizar el manejo de paquetes y dependencias realizado por npm.
	El manejo de paquetes y dependencias que realiza npm es muy parecido al del pom.xml, su nombre es package.json y tiene toda la informacion del programa con el que podemos correrlo al utilizar npm

9)
	Cookiecutter: es una herramienta de CLI desarrollada en Python, que permite crear templates de proyectos.
	make: permite organizar los archivos de compilacion automaticamente, encargandose de la gestion de dependencias.
	pip: permite instalar y administrar paquetes en Python.

10)
	maven->java
	Jenkins->servers
	pipenv->python
	nAnt->.Net
	Ant->java
	Phing->php
	Grung->js
	gulp->js
	Sbt->Scala