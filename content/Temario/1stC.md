> [!Tip]
> Lectura Recomendada 👌: [C vs. Java, Types, Reading and Writing](https://www.cs.helsinki.fi/group/cpro/c1-bea_13.pdf)

# Primer Ejemplo

Fundamentos C. Ejemplo _**1st.c**_ [Click aquí](https://mega.nz/#!mZ1gQY6a!d_QOiIWx6d7mfnwEdS_ehQczOet5NgSL7YDy_UWOEu0)

### Secuencia de compilación [[gcc]]
- Fichero fuente => editor de archivos (programas)
- Compilación => compilador [[gcc]] para general el objeto (código compilado)
- Ejecución => binario, código ejecutable. Ojo a los permisos en Linux
- Ejemplos de órdenes de compilación en el fichero _compilar.txt_

### Bloques de programas
- Includes, librerías. Definición de macros
- Declaración (ojo, distinto de definición) de variables y funciones
- Definición de funciones. Código
- Función main. Argumentos de programa

# Segundo Ejemplo: Introducción I/O

#### int printf(const char *format, ...)

- [https://www.tutorialspoint.com/c_standard_library/c_function_printf.htm](https://www.tutorialspoint.com/c_standard_library/c_function_printf.htm)

#### int fprintf(FILE *stream, const char *format, ...)

- [https://www.tutorialspoint.com/c_standard_library/c_function_fprintf.htm](https://www.tutorialspoint.com/c_standard_library/c_function_fprintf.htm)

#### int scanf(const char *format, ...)

- [https://www.tutorialspoint.com/c_standard_library/c_function_scanf.htm](https://www.tutorialspoint.com/c_standard_library/c_function_scanf.htm)

### Claves del ejercicio
- Abrir en el editor el archivo _**main.c**_ en carpeta **_Ej1printf_**
- Declaración vs Definición
- Uso de **_printf/fprintf_**? Para algo está el manual: **_man 3 printf_**
- Argumentos de main. Paso de parámetros a los programas

# Tercer Ejemplo

> [!Info]
> Este ejercicio contiene elementos, por ejemplo, punteros en los argumentos en la línea de orden que aún no se han visto. Por tanto, por ahora lo relevante del ejemplo es que se trata del primer caso donde interviene más de un fichero fuente como también va a ocurrir en los ejercicios de las prácticas. Por consiguiente, la compilación de los mismos va a resultar algo más compleja puesto que se han de compilar y montar todos los ficheros que componen la "aplicación"
> 

La siguiente línea de orden compila los dos ficheros fuente (**_auxiliar.c_** y **_ejBase.c_**) y monta el ejecutable **_ejBase_**


```shell
gcc -Wall auxiliar.c ejBase.c -o ejBase
```

Descargar los fuentes de _**ejBase**_ [aquí](https://mega.nz/#!jB1D2A5Q!F1KoCf5KRkCPlEVYmGhL92JgoBKbKR7Yp0_F2rKEfDM)

# Ejercicios propuestos

1. Reorganizar los fuentes del segundo ejemplo para que el código de _**MiFuncion()**_ esté en un archivo fuente separado llamado _**MiFuncion.c**_ Es decir, la solución final requiere 2 archivos .c
2. Escribir un programa _**echo.c**_ que partiendo de 1st.c escriba en pantalla un texto que lee de teclado invocando _**scanf()**_ como en el [ejemplo en tutorialspoint](https://www.tutorialspoint.com/c_standard_library/c_function_scanf.htm):

```c
#include <stdio.h>

int main () {
   char str1[20], str2[30];

   printf("Enter name: ");
   scanf("%19s", str1);

   printf("Enter your website name: ");
   scanf("%29s", str2);

   printf("Entered Name: %s\n", str1);
   printf("Entered Website:%s", str2);
   
   return(0);
}
```