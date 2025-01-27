# Parte a
Para descargar una imagen se utiliza: docker pull "imagen" y se descarga la imagen oficial. Para decargar otra version o que este basada en otra se utiliza : y quedaria docker pull nginx:alpine
# Parte b
Alpine esta enfocado a usarse con contenedores (como docker) y es mas liviano. Ubuntu por otra parte esta mas enfocado a desarrolladores y es mas pesada ya que cuenta con paquetes preinstalados
# Parte c
Se usa el comando docker images para ver todas las imagenes disponibles
# Parte d
```bash
echo "Lista de imagenes instaladas"
docker images | sort -k5 | awk {'print $1, $2, $5'} 
```
# Parte e
Se usa el comando docker run "imagen" para correr una imagen ya descargada (si no esta descargada, la descarga). Para asignar los puertos se agrega un -p y se agrega los puertos.
# Parte f
Para hacerlo seria lo siguente: docker stop "container" && docker rm "container" para eliminarlo, el && sirve para que el segundo corra solo si el primer comando se ejecuto con exito. En caso de que no importe el resultado
se usa ; y por ultimo para ejecutar 2 comando en segundo plano es &
# Parte g
El comando stop detiene un container que este corriendo; el comando rm elimina el container, siempre y cuando este no este corriendo.
# Parte h
Para eliminar imagenes que no esten en uso se utiliza: docker rmi "imagen o id". Importante: La imagen se borra solo si no hay container corriendo en la misma.
