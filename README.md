# desarrollo_local
Creación de contenedores para crear un ambiente local de desarrollo con Docker, usando servicios de Traefik, phpMyadmin, MySQL y Apache (con PHP).


Se debe dar 777 a la carpeta de data de mysql
Es necesario crear una carpeta vacia en html dentro de volumes de apache para crear el proyecto que se quiera trabajar.

docker run --rm --interactive --tty --volume $PWD/apache/volumes/html:/app composer create-project symfony/website-skeleton web 

docker run --rm --interactive --tty --volume $PWD:/app composer create-project symfony/website-skeleton mi_proyecto --ignore-platform-reqs --no-scripts

docker run --rm --interactive --tty --volume $PWD/apache/volumes/html/web:/app composer install --ignore-platform-reqs --no-scripts
