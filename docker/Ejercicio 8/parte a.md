# Seguridad en Docker

Parte a:

Se puede usar un dockerfile para definir el usuario a usar o usando --user id_user:id_grupo cuando se usa un run

Parte b:

Se usa -m o --memory mas la cantidad que se quiere limitar con la memoria y --cpus para el CPU 

Parte c:

Hay varias practicas de seguridad para Docker, algunas de ellas son:

1- Siempre usar imagenes oficiales y confiables (como Docker hub) y evitar usar la version latest ya que no siempre es la mas segura, imagenes como alpine son mas livianas y seguras. Tambien es bueno mantener actualizado Docker

2- Limitar los puertos utilizados con redes personalizadas y evitar guardar contraseñas en dockerfile.

3- Usar apps de monitoreo para registrar actividad sospechosa como Prometheus
