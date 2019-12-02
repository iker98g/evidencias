# 3. Gestión de DNS

Nos meteremos en GUEBS, donde tenemos creado un hosting compartido llamado dominios.fpz1920.com. A través del panel de este hosting crearemos el vínculo entre un nuevo subdominio y nuestra instancia en EC2. 

Para ello, entraremos dentro de registros DNS e ingresaremos los datos nombrados a continuación.

![](images/tarea-3/gestion_dns_1.PNG)

El nombre de mi subdominio será iker.dominios.fpz1920.com. El TTL será 300 como bien viene por determinado. El tipo será A, ya que queremos apuntar nuestro dominio hacia un servidor que tenga una dirección IP estática. Y la dirección será la IP Elastica que hemos reservado y asociado en la tarea anterior.

![](images/tarea-3/gestion_dns_2.PNG)

Una vez rellenado los datos, podremos verlos al final de la página donde tenemos todos los subdominios.

![](images/tarea-3/gestion_dns_3.PNG)








