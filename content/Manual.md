# Utilizar las páginas del manual
```shell
$ man nombre_de_página
```

Los manuales se ordenan en **secciones**:

1. Comandos generales
2. Llamadas al sistema (funciones proveídas por el **kernel**)
3. Llamadas a librerías (funciones de la **librería de C**)
4. Ficheros especiales (normalmente se encuentran /dev) y controladores
5. Formatos de archivos y convenciones
6. Juegos
7. Miscelánea (incluye convenciones)
8. Comandos de administración de sistemas (normalmente requiere privilegios de superusuario) y demonios

## Librería vs Kernel

OJO, no confundir las líbrerías C con las funciones del kernel. Aunque esta cuestión es más propia de sistemas operativos, basta con tener en cuenta lo siguiente:

- en la práctica del programador (la asignatura) no hay necesidad de distinción alguna. Kernel y librería C proveen conjuntamente todos los servicios que necesita
- las funciones de la librería se pueden ver como programas que otros programadores han escrito para facilitarnos la vida (no repetir el mismo programa)
- en último extremo, las funciones de la librería invocan los servicios del kernel
- la librería oculta los detalles de cada sistema en particular que quedan confinados en el kernel. Es decir, la librería es la misma para cualquier sistema UNIX, en particular, cualquier distro Linux
```shell
man S keyword
```
Generalmente, para indicar las páginas del manual se suelen usar el nombre seguido del número entre paréntesis de la sección a la que pertenece. A menudo, existen múltiples páginas del manual con el mismo nombre, como *man(1)* y *man(7)*. Por ejemplo, para leer la página del manual sobre */etc/passwd*, en vez de la página sobre el propio comando *passwd*:

```shell
$ man 5 passwd
```
## Whatis

Descripciones de una línea de las páginas del manual pueden mostrarse usando el comando *whatis*. Por ejemplo, para una breve descripción de las páginas de secciones del manual sobre *printf*:
```shell
santiago@Folio13:~$ whatis printf  
printf (3) - formatted output conversion  
printf (1) - format and print data
```
