# Instalación de Moodle

Actualizamos el equipo, se trata de una Xenial, así que vemos cual es la versión disponible de Moodle que se encuentra en los repositorios.

 *`apt-cache show moodle`
 
Vemos que se trata de una versión 3.0.3 y para poder estar un poquito más actualizados, vamos a intentar descargar de la página oficial del proyecto la versión 3.3 de Moodle.

Al hacer esto, debemos tener en cuenta que actualizaremos de manera "Manual" con sus *pros* y sus *contras*.
#TODO 

Descargamos la última versión (en este momento la 3.3)


`axel https://download.moodle.org/download.php/direct/stable33/moodle-3.3.tgz`

Nos vamos a la carpeta /srv/ y descomprimimos el tgz en moodle-3-3, y creamos un enlace a moodle. 

 `$ cd /srv`
 `$ mv moodle moodle-3-3`
 `$ ln -s moodle-3-3 moodle`
 
Creamos un site en `/etc/apache/sites-avaliable/` por ejemplo `/etc/apache/sites-avaliable/moodle.conf`

