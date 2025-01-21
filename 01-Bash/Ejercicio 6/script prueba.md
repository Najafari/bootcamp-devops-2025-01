Version 0.1
```bash
#!/bin/bash

# Parte a: Listar IPs y hostnames
Function rIPs () {
echo -e "Presione enter para listar todas las IPs y host"
read enter1
awk '$1 ~ /^192\.168/ {print $0}' archivo.conf
}

# Parte e: eliminar entradas
Function rDelete () {
echo "Escriba aqui el nombre de la entrada a eliminar:"
read deleteentry
sed -i '$deleteentry/d' archivo.conf
}

# Parte f: Modificar entradas
Function rModify () {
echo "Escriba aqui el nombre de la entrada a editar:"
read oldmod
echo "Escriba auqi el nombre de la entrada nueva:"
read newmod
sed -i 's/$oldmod/$newmod/g' archivo.conf

echo "Entrada modificada!"
}

# Esto es el menu
Function menu () {
while true; do
clear
	echo -e "Selecciona lo que quieras hacer a continuacion\n"
	echo -e "1) Listar IPs y hostnames"
	echo -e "2) Eliminar entrada"
	echo -e "3) Modificar entrada"

read -p "Ingrese la opcion:" choice

case $choice in
1) rIPs;;
2) rDelete;;
3) rModify;;
*) echo -e "Opcion no valida";;
esac
