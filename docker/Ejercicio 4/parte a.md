# Redes en Docker

Parte a:
docker network create --driver bridge --subnet "ip" --gateway "ip" network_prueba

Parte b:
docker run -d --name container_prueba --network network_prueba alphine

Parte c:
docker network ls

Parte d:
Se hace con un ping. Ej:
docker run -d --name container_1 --network network_prueba alphine

docker run -d --name container_2 --network network_prueba alphine

docker exec -it container_1 sh 

ping container_2

Deberia devolver un ping mostrando que estan conectados

Parte e:
Se utiliza el nombre del container como un hostname cuando los contenedores estan conectados a la misma red. Docker resuelve el Ip con el hostname
