# 5. Servidor FTP

Lo primero que vamos a hacer es habilitar el puerto 21 en el FTP.

![](images/tarea-5/puerto_ftp.PNG)

Paso seguido, instalaremos el FTP en nuestra máquina a través del siguiente comando:

    sudo apt-get install vsftpd

![](images/tarea-5/comando_ftp.PNG)

A continuación, crearemos tres usuarios llamados cliente, servidor y admin en sus respectivos directorios.

![](images/tarea-5/usuarios_2.PNG)

![](images/tarea-5/usuarios.PNG)

Ahora editaremos al archivo FTP.

![](images/tarea-5/comando_ftp_2.PNG)

Y escribimos las siguientes líneas.

![](images/tarea-5/comando_ftp_3.PNG)

Reiniciamos y habilitamos el servicio ftp.

![](images/tarea-5/comando_ftp_4.PNG)

Entramos en WinSCP y nos conectamos con el usuario admin.

![](images/tarea-5/winscp_2.PNG)

Desactivamos el modo pasivo.

![](images/tarea-5/winscp.PNG)

Y comprobamos que todos los pasos los hemos hecho bien.

![](images/tarea-5/winscp_3.PNG)