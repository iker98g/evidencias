# 3. Instalación.

- [Actualizar lista de paquetes](#actualizar-lista-de-paquetes)

- [Instalar Apache](#instalar-apache)

- [Instalar MySQL](#instalar-mysql)

## Actualizar lista de paquetes

Vamos a ejecutar el siguiente comando para tener actualizada la lista de paquetes en su ultima versión:

    sudo apt-get update

![](images/tarea-2/listado_de_paquetes.PNG)

## Instalar Apache

El siguiente paso será la instalación del Apache en nuestra máquina virtual. Para ello, ejecutaremos el siguiente comando:

    sudo apt install apache2

Una vez ejecutado el comando, nos preguntará a ver si queremos continuar, le respondemos que si y se instalará Apache.

![](images/tarea-2/instalacion_apache.PNG) 

## Instalar MySQL

A continuación, instalaremos MySQL. MySQL es un sistema de gestión de bases de datos de código abierto. Lo instalaremos de la siguiente forma:

    sudo apt install mysql-server

![](images/tarea-2/instalacion_mysql.PNG)

#### Configurar MySQL

Esto instalará MySQL, pero no nos pedirá que creemos ninguna contraseña ni que hagamos ningún otro cambio de configuración. Dado a que esto deja su instalación de MySQL insegura, vamos a ejecutar el siguiente script de seguridad:

    sudo mysql_secure_installation

![](images/tarea-2/configuracion_mysql_1.PNG)

Al ejecutar este comando, nos mandará una serie de preguntas sobre la contraseña, usuario, privilegios... Respondemos todas las preguntas y ya tendremos el MySQL configurado.

![](images/tarea-2/configuracion_mysql_2.PNG)

Escribiendo el siguiente comando entraremos dentro del MySQL

    sudo mysql

![](images/tarea-2/configuracion_mysql_3.PNG)


