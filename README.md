# Creando-usuarios-y-grupos-
se explicara paso a paso como crear usuarios y grupo

-Entrar con usuario root
-para crear usuario utilizamos en comando useradd, lo utilizaremos asi
**useradd marina**
**useradd yesy**
 ya creamos los usuarios los verificamos con este comando: **nano /etc/passwd**   se da Ctrl + x para salir
-se le pone contraseña a los usuarios con el siguente comando passwd + en nombre de usuario
 **passwd marina**   
pedira que escribas una contaseña, luego pide que la vuevas a escribir la contraseña
se hace lo mismo con este usuario **passwd yesy** 
es su desicion si lo dejas con la misma contraseña en los dos usuario
se verifican las contraseñas con este comando: **nano /etc/shadow:
-lo siguiente es grear el grupo con el comando groupadd asi: **groupadd casa**
se verifica con el comando: **cat /etc/gropu**
-agregar los usuarios al grupo con el comando adduser asi:
**adduser marina casa**
**adduser yesy casa**
verificar los usuarios del grupo con el comando getent asi: **getent group casa**
-cambiar el nombre del grupo con el comando groupmod asi:
**groupmod**  se le da enter y le apareceran una opciones, como lo que queremos es cambiar de nombre seria el -n asi:
**groupmod -n familia casa**
se verifica con el comando: **cat /etc/gropu**
eso sera todo
