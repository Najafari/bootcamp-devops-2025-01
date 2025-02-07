# Docker Compose

Parte a:

Seria:

```bash
Version: 1
  Services:
    image: alphine
    ports:
      - host:contenedor
    volumes:
      - volumen_prueba:ruta/contenedor
    networks:
      - nerwork_prueba
  Otro servicio:
    imagen: alphine
    links:
     - redis
```

Parte b:

Primero te ubicas en el directorio donde esta el compose y le das docker-compose up

Parte c:
docker-compose ps

Parte d:

docker-compose down

Parte e:

docker-compose down detiene y elimina todo mientras que docker-compose stop simplemente 
     
