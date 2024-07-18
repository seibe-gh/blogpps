# Conexión remota
Por ejemplo, desde nuestro linux personal: 
```bash
ssh usuario@triqui1.fi.upm.es
```
Esto nos abre una shell _**bash**_ desde la cual empezar a emitir comandos. Para salir **exit** o **^D**

Si se desea ==se puede configurar ssh para que no sea necesario introducir la contraseña==. Para ello es necesario generar e instalar un par de claves. El proceso se describe muy claramente [aquí](https://www.ochobitshacenunbyte.com/2019/03/13/ssh-sin-contrasena-en-linux/)

# Carpeta home o personal del usuario

> [!Danger]
> <font color="#ff0000">Comprobar **permisos**</font> (estamos en un sistema multiusuario)!!!

```bash
ls -ld $HOME
```
La salida debe mostrar:
`drwx------`
Para editar ficheros fuente .c necesitamos, obviamente, un editor: _**vi**_ y/o _**nano**_

> [!Info] Permisos y más
> Contents
