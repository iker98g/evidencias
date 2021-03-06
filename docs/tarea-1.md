# 1. Conectarse mediante SSH al servidor Ubuntu de AWS.

- [Conectarse vía SSH para comprobar conectividad](#conectarse-via-ssh-para-comprobar-conectividad)

## Conectarse vía SSH para comprobar conectividad

Para conectarnos mediante SSH a nuestro servidor Ubuntu de Amazon Web Services haremos lo siguiente: 

Vamos a la consola y nos colocamos dentro de la carpeta donde tenemos la llave pública.

Y acontinuación, escribimos el siguiente comando en el terminal:

    ssh -i "awsiker.pem" ubuntu@ec2-107-22-130-22.compute-1.amazonaws.com

![](images/tarea-1/conexion_via_ssh.PNG)

# Instalación.

- [Actualizar lista de paquetes](#actualizar-lista-de-paquetes)

- [Instalar Apache](#instalar-apache)

- [Instalar MySQL](#instalar-mysql)

- [Instalar phpMyAdmin](#instalar-phpmyadmin)

## Actualizar lista de paquetes

Vamos a ejecutar el siguiente comando para tener actualizada la lista de paquetes en su ultima versión:

    sudo apt-get update

![](images/tarea-1/listado_de_paquetes.PNG)

## Instalar Apache

El siguiente paso será la instalación del Apache en nuestra máquina virtual. Para ello, ejecutaremos el siguiente comando:

    sudo apt install apache2

Una vez ejecutado el comando, nos preguntará a ver si queremos continuar, le respondemos que si y se instalará Apache.

![](images/tarea-1/instalacion_apache.PNG) 

## Instalar MySQL

A continuación, instalaremos MySQL. MySQL es un sistema de gestión de bases de datos de código abierto. Lo instalaremos de la siguiente forma:

    sudo apt install mysql-server

![](images/tarea-1/instalacion_mysql.PNG)

#### Configurar MySQL

Esto instalará MySQL, pero no nos pedirá que creemos ninguna contraseña ni que hagamos ningún otro cambio de configuración. Dado a que esto deja su instalación de MySQL insegura, vamos a ejecutar el siguiente script de seguridad:

    sudo mysql_secure_installation

![](images/tarea-1/configuracion_mysql_1.PNG)

Al ejecutar este comando, nos mandará una serie de preguntas sobre la contraseña, usuario, privilegios... Respondemos todas las preguntas y ya tendremos el MySQL configurado.

![](images/tarea-1/configuracion_mysql_2.PNG)

Escribiendo el siguiente comando estaremos dentro de MySQL:

    sudo mysql

![](images/tarea-1/configuracion_mysql_3.PNG)

## Instalar phpMyAdmin

Como último paso, vamos a instalar phpMyadmin para poder acceder a las BBDD:

![](images/tarea-1/instalacion_phpmyadmin_1.PNG)

Cuando comience la instalación, obtendremos el siguiente mensaje que nos pedirá que seleccionemos el servidor web, nosotros seleccionaremos apache2.

![](images/tarea-1/instalacion_phpmyadmin_2.PNG)

En la siguiente pantalla, pedirá que la base de datos sea utilizada por phpMyAdmin. Lo dejaremos por defecto.

![](images/tarea-1/instalacion_phpmyadmin_3.PNG)

Por último, introduciremos una contraseña para acceder a phpMyAdmin y la confirmaremos nuevamente en la siguiente pantalla.

![](images/tarea-1/instalacion_phpmyadmin_4.PNG)





