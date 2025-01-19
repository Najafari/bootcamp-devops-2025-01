# Copia de Archivos por Fecha de Modificación
```bash
find /var/log -newermt "2025-01-08" ! -newermt "2025-01-09" -exec cp {} /desk/copia_1 \;
