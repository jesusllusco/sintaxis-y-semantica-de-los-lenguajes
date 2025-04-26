# TP N°0: Hello World
[![C-Logo](https://disenowebakus.net/imagenes/articulos/lenguaje-de-programacion-c.jpg "C")](https://disenowebakus.net/imagenes/articulos/lenguaje-de-programacion-c.jpg "C")

## Datos requeridos

### Compilador

El compilador utilizado para este trabajo práctico es **GCC (GNU Compiler Collection)**

[![GCC-Logo](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSVlNOLXqtq1RWiPQaDaY3Rf4_h8GutepeQtg&s)](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSVlNOLXqtq1RWiPQaDaY3Rf4_h8GutepeQtg&s)


### Versión de compilador

La versión del compilador puede verificarse mediante el siguiente comando por cmd de Windows:
- `gcc --version`

En mi caso la versión instalada es la 6.3.0

[![gcc-version-screenshot](https://raw.githubusercontent.com/jesusllusco/sintaxis-y-semantica-de-los-lenguajes/refs/heads/main/00-chelloworld/assets/gc-version-screenshots.png)](https://raw.githubusercontent.com/jesusllusco/sintaxis-y-semantica-de-los-lenguajes/refs/heads/main/00-chelloworld/assets/gc-version-screenshots.png)

### Versión del standard de C

La versión del standard de C utilizada por GCC puede verificarse por medio del siguiente comando en CMD de Windows:
- `gcc -dM -E - < NUL | findstr __STDC_VERSION__`

En mi caso tengo instalado C11.

[![standard-c11-screenshot](https://raw.githubusercontent.com/jesusllusco/sintaxis-y-semantica-de-los-lenguajes/refs/heads/main/00-chelloworld/assets/standard-c-screenshot.png "standard-c11")](https://raw.githubusercontent.com/jesusllusco/sintaxis-y-semantica-de-los-lenguajes/refs/heads/main/00-chelloworld/assets/standard-c-screenshot.png "standard-c11")




