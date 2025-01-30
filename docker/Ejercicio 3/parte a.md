# Creación de un Dockerfile

para crear un Dockerfile se tiene que tener: FROM que sera el que especifique el sistema operativo, actualizar/instalar los repositorios y dependencias necesarias, agregar el COPY para el codigo fuente y un ENTRYPOINT para saber que comando se debe correr cuando comience la imagen

Parte a:

para construir un imagen personlizada usando un dockerfile usaria: "docker build . -t "nombre de la imagen:flag"

Parte b:

Se puede usar 2 metodos: inspect o compose. Para inspect seria "docker inspect "imagen"" donde se vera con detalle el arranque de la imagen y otros detalles; Sino se puede usar compose "docker-compose -up --build" si todo levanta la imagen esta bien.

Parte c:

docker run -it --name "container personalizado" "nombre de la imagen"

Parte d:

COPY sirve para copiar archivos desde un punto a otro, mientras que ADD se usa para copiar y descomprimir o para descargar desde una URL. En caso de solo querer copiar usar COPY si se quiere descomprimir usar ADD

Parte e:

Entrypoint es un comando especifico que debe correr la imagen luego de comenzar, RUN permite ejecutar comandos dentro de un container y CMD
