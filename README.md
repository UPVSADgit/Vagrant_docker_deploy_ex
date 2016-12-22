

Os proporciono una versión que no ejecuta el docker-compose en el provisioning. Esto es para que apreciéis mejor el funcionamiento de
docker-compose up.

Deberéis entrar en una sesión ssh, y en el directorio /vagrant/service ejecutar el comando docker-compose up.

docker-compose os muestra los comandos disponibles si no le pasáis ninguno. Tiene opciones para pausar, reanudar, matar, inspeccionar, etc.. cada uno de los componentes creados (pero siempre ejecutándolo en la carpeta donde está el fichero docker-compose.yml)

por ejemplo: docker-compose kill service_wor_1

Para escalar los componentes se puede usar el comando docker-compose scale. Por ejemplo, dentro de la carpeta /vagrant/service, si le especificamos docker-compose scale cli=10, creará 10 nuevos componentes clientes.

para matar los contenedores podéis usar también docker kill nombre_contenedor
