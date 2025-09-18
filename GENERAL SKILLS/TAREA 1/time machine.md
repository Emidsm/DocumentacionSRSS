
### Descripción del Reto

La bandera está oculta en una versión anterior de un repositorio de Git.

### Procedimiento (Paso a Paso)

1. Cloné el repositorio y usé `git log --oneline` para ver un resumen del historial.
    
2. Los mensajes de los commits no daban muchas pistas, así que decidí probar los commits anteriores.
    
3. Usé `git checkout HEAD~1` para ir al commit anterior al actual, y el archivo `flag.txt` apareció.
    
4. Leí el contenido con `cat`.
    

### La Bandera

`picoCTF{t1m3_m4ch1n3_938c4b}`