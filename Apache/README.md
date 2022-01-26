## Instalar dependencias
Instalar dependencias de proyectos de laravel con composer. 

    docker run --rm --interactive --tty --volume $PWD:/app  composer install --ignore-platform-reqs --no-scripts

Para habilitar la extensión mysqli es necesario crear una imagen e instalar el paquete usando

docker-php-ext-install mysqli
