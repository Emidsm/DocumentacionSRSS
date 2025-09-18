
### Descripción del Reto

Encontrar la bandera que está oculta en un archivo relacionado con las tareas programadas en el sistema.

### Procedimiento (Paso a Paso)

1. Utilicé `crontab -l` para ver si había tareas programadas a nivel de usuario, pero no encontré nada.
    
2. Me di cuenta de que los archivos de cron del sistema a menudo están en el directorio `/etc/cron.d`.
    
3. Usé `ls -la /etc/cron.d` y encontré un archivo sospechoso.
    
4. El contenido de ese archivo me dio la pista para encontrar la bandera en un directorio temporal.
### La Bandera

`picoCTF{c4n_y0u_s33_th3_t1m3_934d7d}`