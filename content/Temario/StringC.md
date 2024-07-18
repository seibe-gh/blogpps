---
title: StringC
draft: "true"
---

> [!Info] Notas previas
> - Ejercicio ultra sencillo sobre arrays y strings en C
>- Se presupone **dominio de estructuras iterativas (bucles) y arrays (en el lenguaje que sea y, en particular, en Java)**
>- También se ven las funciones de librería ***printf()***, ***scanf()***, ***fgets()***, ***strcpy()*** y ***strcat()***
>- Declaración de tipos: _**[typedef](https://www.tutorialspoint.com/cprogramming/c_typedef.htm)**_
>- En todo caso, se recomienda revisar la documentación de todas las funciones (librerías del sistema) utilizadas en el ejercicio

![String Presentation in C/C++](https://www.tutorialspoint.com/cprogramming/images/string_representation.jpg)

## Lecturas recomendadas
- [C-Strings](https://www.tutorialspoint.com/cprogramming/c_strings.htm)
- [C Library - <string.h>](https://www.tutorialspoint.com/c_standard_library/string_h.htm)
- [ANSI C String Library](https://download.mikroe.com/documents/compilers/mikroc/pic32/help/ansi_string_library.htm)
- [C – Strings and String functions with examples](https://beginnersbook.com/2014/01/c-strings-string-functions/)
- Referencias [<stdio.h>](https://www.tutorialspoint.com/c_standard_library/stdio_h.htm) y [<stdlib.h>](https://www.tutorialspoint.com/c_standard_library/stdlib_h.htm)
### Enlace de descarga pulsando aquí: [StringC.zip](https://mega.nz/#!vcdnTIRQ!5jx7cYwMo3G01QIXsECIZvVO_kV5yT7KQsAYyubY8cc)
### COMPILACIÓN
- Compilar: `gcc -c -o StringC.o StringC.c`
- Montar: `gcc -o StringC ./StringC.o`
> [!Info]
> Consultar el manual de gcc: man gcc (man info)
## TAREAS
### 1ª Parte
Completar función catstr1()
### 2ª Parte
En la función main del programa se invocan las cuatro funciones implementadas. Cada una corresponde con un test diferente. Para testear de manera unitaria debería haber un main diferente para cada test. Por tanto, se pide:
1. Crear un StringC.h con todas las cabeceras (declaraciones) de las funciones en StringC.c
2. Crear un programa de test para cada caso. Por ejemplo, test1.c
3. Compilar y ejecutar por separado cada test
