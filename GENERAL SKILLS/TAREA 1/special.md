
### Descripción del Reto

La bandera se encuentra dentro de un shell especial y restringido, y el objetivo es encontrar una manera de escapar para poder ejecutar comandos de Linux normales.

### Procedimiento (Paso a Paso)

1. Intenté ejecutar comandos simples como `ls` y `cat`, pero fueron bloqueados.
    
2. Me di cuenta de que el shell restringido no validaba los caracteres especiales.
    
3. Usé el punto y coma `;` para encadenar un comando permitido con un comando no permitido, como `echo "test"; ls -l`. Esto me permitió ver el contenido del directorio.
    
4. Descubrí un script llamado `get_flag.sh` y lo ejecuté para obtener la bandera.
    

### La Bandera

`picoCTF{3sc4p3_th3_ch4r4ct3r_5h3ll_93b22}`