# TP N°0: Hello World

[![C-Logo](https://disenowebakus.net/imagenes/articulos/lenguaje-de-programacion-c.jpg  "C")](https://disenowebakus.net/imagenes/articulos/lenguaje-de-programacion-c.jpg  "C")

  

## Información requerida

### Compilador

El compilador utilizado para este trabajo práctico es **GCC (GNU Compiler Collection)**

[![GCC-Logo](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSVlNOLXqtq1RWiPQaDaY3Rf4_h8GutepeQtg&s)](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSVlNOLXqtq1RWiPQaDaY3Rf4_h8GutepeQtg&s)

### Versión de compilador

La versión del compilador puede verificarse mediante el siguiente comando por cmd de Windows:

-  `gcc --version`

En mi caso la versión instalada es la 6.3.0

[![gcc-version-screenshot](https://raw.githubusercontent.com/jesusllusco/sintaxis-y-semantica-de-los-lenguajes/refs/heads/main/00-chelloworld/assets/gc-version-screenshots.png)](https://raw.githubusercontent.com/jesusllusco/sintaxis-y-semantica-de-los-lenguajes/refs/heads/main/00-chelloworld/assets/gc-version-screenshots.png)

### Versión del standard de C

La versión del standard de C utilizada por GCC puede verificarse por medio del siguiente comando en CMD de Windows:

-  `gcc -dM -E - < NUL | findstr __STDC_VERSION__`

En mi caso tengo instalado C11.

[![standard-c11-screenshot](https://raw.githubusercontent.com/jesusllusco/sintaxis-y-semantica-de-los-lenguajes/refs/heads/main/00-chelloworld/assets/standard-c-screenshot.png  "standard-c11")](https://raw.githubusercontent.com/jesusllusco/sintaxis-y-semantica-de-los-lenguajes/refs/heads/main/00-chelloworld/assets/standard-c-screenshot.png  "standard-c11")

## Resultados paso a paso

### Código fuente

El presente TP cuenta con un archivo llamado **hello.c** el cual se encargará de imprimir el siguiente texto por consola:

> hola mundo!!!

 El archivo contiene el siguiente código:
 
    #include <stdio.h>
    int main()  {
		printf("Hola mundo!!!\n");
		return  0;
	}

 ### Compilación

Para compilar el archivo fuente se debe ejecutar el siguiente comando por CMD en Windows:

 - `gcc nombreArchivo.c -o nombrePrograma.exe`

Este comando hace uso de la opción `-o nombrePrograma.exe` el cuál no dará como resultado la creación de un archivo llamado **nombrePrograma.exe** el cuál representa el archivo ejecutable que utilizaremos para correr el programa.

En mi caso como mi archivo se llama **hello.c** el comando que he utilizado es `gcc hello.c -o hello.exe`, como se ve en la siguiente imagen.

![enter image description here](https://raw.githubusercontent.com/jesusllusco/sintaxis-y-semantica-de-los-lenguajes/refs/heads/main/00-chelloworld/assets/file-compile-screenshot.png)

Obteniendo como resultado el siguiente archivo:

![enter image description here](https://raw.githubusercontent.com/jesusllusco/sintaxis-y-semantica-de-los-lenguajes/refs/heads/main/00-chelloworld/assets/file-compile-out-sreenshot.png)

### Ejecución archivo .exe

Al obtener el archivo `nombrePrograma.exe`este debe ser ejecutado para poder ver el resultado del programa. Para ello hay dos formas de hacerlo.

 1. Hacer doble clic izquierdo sobre el ícono del archivo.
 2. Ejecutar por consola de CMD en Windows, el siguiente comando: 
 `./nombrePrograma.exe` o directamente `nombrePrograma.exe`

Aclaración: El probable que al intentar ejecutar el archivo .exe mediante la opción 1 no se vea el resultado. Esto es por que el programa se abre, ejecuta y se cierra de inmediato. Se recomienda utilizar la opción 2.

Para este TP utilice el siguiente comando y con siguiente resultado

![resultado-archivo-exe](https://raw.githubusercontent.com/jesusllusco/sintaxis-y-semantica-de-los-lenguajes/refs/heads/main/00-chelloworld/assets/resultado-salida-exe.png)

### Redirección a .txt

Para obtener el texto resultado en un archivo de texto plano en lugar de la CMD podemos utilizar el siguiente comando:

 - `./nombrePrograma.exe > nombreArchivoTexto.txt`

Luego de ejecutado el comando aparecerá en el mismo directorio el archivo llamado **nombreArchivoTexto.txt**

En mi caso el comando le he utilizado del siguiente modo:

![redireccion-txt](https://raw.githubusercontent.com/jesusllusco/sintaxis-y-semantica-de-los-lenguajes/refs/heads/main/00-chelloworld/assets/redireccion-cmd-screenshot.png)

Y el archivo obtenido es:

![redireccion-salida-txt
](https://raw.githubusercontent.com/jesusllusco/sintaxis-y-semantica-de-los-lenguajes/refs/heads/main/00-chelloworld/assets/redireccion-out-screenshot.png)

### Ver resultados del archivo de texto

Al obtener el archivo `nombreArchivoTexto.txt`este debe ser ejecutado para poder ver el resultado del programa. Para ello hay dos formas de hacerlo.

 1. Hacer doble clic izquierdo sobre el ícono del archivo.
 2. Ejecutar por consola de CMD en Windows, el siguiente comando: 
 `type nombreArchivoTexto.txt`

Para mi TP los resultados con cada método serían los siguientes:

 
 1. Doble clic izquierdo sobre ícono:
![resultado-archivo-texto-txt
](https://raw.githubusercontent.com/jesusllusco/sintaxis-y-semantica-de-los-lenguajes/refs/heads/main/00-chelloworld/assets/resultado-salidatxt-screenshot.png)
 
 2. Por CMD en Windows:
 ![resultado-cmd-txt
 ](https://raw.githubusercontent.com/jesusllusco/sintaxis-y-semantica-de-los-lenguajes/refs/heads/main/00-chelloworld/assets/resultado-salida-screenshot.png)

