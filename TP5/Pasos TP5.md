Ing. de Soft. III
TP5

3)
-Que es Maven?
	Es una herramienta de gestion de proyectos, simplifica procesos de build, sin la necesidad de proecuparse de los modulos,
 dependencias y librerias que necesite el proyecto

-Que es el archivo POM?
	La unidad básica de trabajo en Maven es el llamado Modelo de Objetos de Proyecto conocido simplemente como POM 
(de sus siglas en inglés: Project Object Model).
	Se trata de un archivo XML llamado pom.xml que se encuentra por defecto en la raíz de los proyectos y que contiene 
toda la información del proyecto: su configuración y sus dependencias.
	
	-modelVersion: Define la version de Maven que utiliza el proyecto
	-groupId: Define el nombre de la libreria
	-artifactId: Define el nombre del proyecto, del target a generar
	-versionId: Define la version de la libreria que se esta desarrolando

-Repositorios
	
	-Local: El repositorio local es un directorio en la computadora donde se ejecuta Maven. ALmacena en cache las descargas 
remotas y contiene artefactos de compilacion.
	-Central: Por defecto se buscan las dependencias que se necesiten en este repositorio, global y publico.
	-Remoto: Los repositorios remotos se refieren a cualquier otro tipo de repositorio, al que se accede mediante una variedad 
de protocolos file:// y https://. Estos repositorios puede ser un repositorio verdaderamente remoto configudaro por un tercero para 
proporcionar sus artefactos para descargar. Otros repositorios "remotos" pueden ser repositorios internos configurados en un servidor 
de archivos o HTTP dentro de su empresa, utilizados para compartir artefactos privados entre equipos de desarrollo y para lanzamientos.

-Ciclo de vida

	-Default, que gestiona la construcción y despliegue del proyecto.
	-Clean, que gestiona la limpieza del directorio del proyecto. Es decir, se encarga de eliminar todos los archivos generados en el proceso de construcción y despliegue.
	-Site, que gestiona la creación de la documentación del proyecto.

