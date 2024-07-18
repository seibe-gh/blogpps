---
title: Edición en remoto
draft: false
---

Los siguientes enlaces muestran los pasos necesarios para configurar marcadores remotos con [Nautilus](https://www.guia-ubuntu.com/index.php/Nautilus):
- [Conectarse a servidor SSH, FTP, SMB desde Nautilus](https://linuxgx.blogspot.com/2016/05/tip-conectarse-servidor-ssh-ftp-sftp.html)
- [Conexión ssh omitiendo la introducción de claves](https://brinchmann.wordpress.com/2014/03/08/tutorial-how-to-use-sftp-with-keys-with-in-nautilus/)
Obviamente, lo anterior requiere un linux funcionando. En [este enlace](https://ubuntu.com/tutorials/create-a-usb-stick-on-windows#1-overview) se describe paso a paso el procedimiento para generar un pendrive con un linux *Ubuntu* arrancable
Otros enlaces que describen el proceso son [este (en español)](https://www.atareao.es/tutorial/linux-mint-cinnamon/crear-un-live-usb-de-linux-en-linux/) y [este otro (en inglés)](https://antergos.com/wiki/es/uncategorized/create-a-working-live-usb/). Existen otras alternativas como son el arranque dual, un sistema de virtualización (VMware, VirtualBox, Docker, etc.) pero esta es, probablemente, la más simple y, sobre todo, la que menos interfiere con el sistema que tengamos instalado y usemos habitualmente
### Copiar ficheros desde/a un servidor remoto
Dos opciones:
1. Instalar [_Filezilla_](https://filezilla-project.org/)
2. Mediante el comando _[scp](https://geekytheory.com/copiar-archivos-a-traves-de-ssh-con-scp)_ (en Windows [_WinSCP_](https://winscp.net/eng/docs/lang:es))