# Listar IPs y Hostnames
```bash
awk '$1 ~ /^192\.168/ {print $0}' archivo.conf
