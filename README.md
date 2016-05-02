# Eclipse


	REPOSITORIO: https://github.com/prodrc02/Eclipse.git



Una vez abierto Eclipse:

1.	Vamos a la pestaña File-New-Java Project
	Damos un nombre al proyecto (en este caso PracticaEclipse) y Finish.
	
2.	Dentro del projecto creado, botón derecho: New-Folder
	A esta carpeta la llamamos lib. Repetimos el paso y la segunda carpeta se llamará etc.
	
	Una vez creadas, dentro de lib copiamos los jar usados en la practica de Log4j; y dentro
	de etc el archivo log4j2.xml
	
3.	En src creamos un paquete, botón derecho: New-Package
	Lo llamamos com.foo
	En este paquete copiamos la clase Bar.java
	
	Y en src copiamos la clase MyApp.java
	
4. 	Hacemos boton derecho en el proyecto: Build Path- Configure Build Path
	Nos situamos en Libraries y luego en Add External JARs y añadimos los .jar que tenemos en la carpeta
	lib del proyecto.
	Una vez añadidas damos a Apply y luego OK.
	
5.	Volvemos  a hacer boton derecho sobre el proyecto y Run As-Run Configurations
	En Classpath vamos a User Entries, y luego Advanced, Add Folders y seleccionamos la carpeta etc del proyecto.
	
	Después damos a Run y se muestra los siguiente:
	
		23:59:58.090 [main] TRACE com.foo.Bar - entry
		23:59:58.090 [main] TRACE com.foo.Bar - entry
		23:59:58.091 [main] ERROR com.foo.Bar - Did it again!
		23:59:58.091 [main] ERROR com.foo.Bar - Did it again!
		23:59:58.092 [main] TRACE com.foo.Bar - exit with(false)
		23:59:58.092 [main] TRACE com.foo.Bar - exit with(false)
		23:59:58.092 [main] ERROR MyApp - Didn't do it.

	
6.	Una vez seguidos todos los pasos, en Github creamos un repositorio con README y conectamos nuestro repositorio
	con el proyecto.
	