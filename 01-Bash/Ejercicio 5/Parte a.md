# Manipulación de Archivos de Texto
```bash
curl -f https://get.docker.com -o install-docker.sh
```
curl -f -- funciona descargando solo si la URL es valida
-o guarda el contenido en un archivo llamado install-docker.sh
```bash
sed -e '316{H;d}' e- '516G'
```
# Usando vim seria mas facil (personalmente)
vim install-docker.sh
yy en la linea 316
dd para borrar la linea 316
P pegar en la linea 516
:wq para guardar y salir
