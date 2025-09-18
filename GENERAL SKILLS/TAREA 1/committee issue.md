
### Descripción del Reto

La bandera fue borrada de un repositorio de Git en un commit anterior.

### Procedimiento (Paso a Paso)

1. Cloné el repositorio de Git con `git clone`.
    
2. Usé `git log` para ver el historial completo de los commits.
    
3. Noté que el commit más reciente tenía un mensaje que decía "Revert: removed flag file".
    
4. Utilicé `git checkout [hash_del_commit_anterior]` para volver al estado del repositorio antes de que la bandera fuera borrada.
    
5. El archivo de la bandera reapareció y pude leerlo con `cat`.
    

### La Bandera

`picoCTF{c0mmitt33_1ssu3s_4r3_c0mm0n_941031}`