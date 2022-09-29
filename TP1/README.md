Ing. de Soft. III

se creo el archivo readme

Trabajo Practico 1

4)
4.1)Pull Request:
	Un Pull Request es una peticion que el propietario de un fork de un repositorio hace al propietario del repositorio original para que este ultimo incorpore los commits que estan en el fork.

4.2)Crear un branch local y agregar cambios a dicho branch.

<img src= "Imagenes TP1/Branch.jpg">

4.3)Subir el cambio a dicho branch y crear un pull request.

4.4)Completar el proceso de revisión en github y mergear el PR al branch
master.

<img src= "Imagenes TP1/PR.jpg">

<img src="Imagenes TP1/Modif1.jpg">


5)
Mensaje colisionado con p4merge

Clonar en un segundo directorio el repositorio creado en github.

<img src="Imagenes TP1/Clon.jpg">

En el clon inicial, modificar el Readme.md agregando más texto.
Hacer commit y subir el cambio a master a github.
En el segundo clon también agregar texto, en las mismas líneas que se modificaron el punto anterior.
Intentar subir el cambio, haciendo un commit y push. Mostrar el error que se obtiene.

<img src="Imagenes TP1/Colision.jpg">

Hacer pull y mergear el código (solo texto por ahora), mostrar la herramienta de mergeo como luce.
Resolver los conflictos del código.

<img src="Imagenes TP1/Pull.jpg">

<img src="Imagenes TP1/Seleccion de archivos.jpg">

<img src="Imagenes TP1/Comparacion desde p4merge.jpg">

Explicar las versiones LOCAL, BASE y REMOTE.

Local: Archivos de la rama actual en el repositorio local de la maquina que se esta utilizando
Remote: Archivos de la rama actual en el repositorio remoto que se esta intentando fusionar en su Local
Base: Los ancestros comunes de Local y Base

6)
Ejercicio Online

<img src="Imagenes TP1/Ejercicio git.jpg">