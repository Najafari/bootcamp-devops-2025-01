# Volúmenes y Persistencia de Datos

Parte a:

docker volume create volumen_prueba

Parte b:

docker run --name mysql_volume -e MYSQL_ROOT_PASSWORD=pass123 -v volumen_prueba:/var/lib/mysql -d mysql

Parte c:

docker volume inspect volumen_prueba

Parte d:

docker volume prune

Parte e:

Usando -v y el nombre del volumen

