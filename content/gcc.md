> [!Warning]
> ## IMPORTANTE: Secuencia típica de compilación

![El proceso de compilación C](https://www3.ntu.edu.sg/home/ehchua/programming/cpp/images/GCC_CompilationProcess.png "El proceso de compilación C")
## Ejemplo de compilación multifuente ([link](https://programacionsistemas.wordpress.com/2011/08/24/1-3-el-gcc/))

Las siguientes órdenes permiten construir un ejecutable a partir de tres archivos fuente y dos librerías

### Compilar bd.c generando objeto bd.o  

```bash
pepito@mihost:~$**gcc** –c bd.c –o bd.o
```

### Compilar motor.c generando objeto motor.o tomando funciones de la librería libgraphics

```bash
pepito@mihost:~$**gcc** –c motor.c –lgraphics –o motor.o
```

### Compilar menu.c generando menu.o tomando funciones de libcurses

```shell
pepito@mihost:~$**gcc** –c menu.c –lcurses –o menu.o 
```

### Montar los tres objetos anteriores en un ejecutable llamado juego

```shell
pepito@mihost:~$**gcc** bd.o motor.o menu.o –o juego
```

