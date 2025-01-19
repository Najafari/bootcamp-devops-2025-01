# Carpeta Más Pesada en un Nivel de Subdirectorios
```bash
du -ah --max-depth=3 / | sort -rh | head -n 1
```
La primera parte busca los archivos con un nivel de estructura 3
La segunda parte organiza los archivos por tamaño
La ultima parte muestra la opcion mas pesada
