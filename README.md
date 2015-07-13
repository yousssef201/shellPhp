# shellPhp

Un ejemplo practico el porque no debes dejar que en tu server HTTP existan archivos con extension PHP con permisos de lectura y escritura y sobretodo con grupos como root o peor aun que el dueño sea root.

Comprometiendo la seguridad en absoluto del servido.

El scrip corre bajo una terminal por lo cual no es necesario correrlo desde el servidor Apache.

Para ejecutar el scrip es necesario proporcionarle 2 parametros, el primero de ellos es el host y el puerto. En un ejemplo practico podriamos correr el scrip de la siguiente manera:

# status.php localhost 444

Donde "localhost" obviamente es el destino donde se pondra a la escucha el puerto, que en este caso es el segundo parametro "444". Siendo asi, el script crea una conexion TCP que permite conexiones entrantes por el puerto 444 sin que este solicite autenticacion o password.

Proximamente se agregaran mas funcionalidades a este scrip.
+ Autenticacion por usuario y/o password
+ Manera de ocultar el puerto local
+ Upload/Download de archivos
+ Navegacion por el arbol de directorios
+ Reverse shell
+ Recepcion de indicaciones mediante IRC
+ etc...
