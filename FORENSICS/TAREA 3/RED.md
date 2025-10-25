RED

- Descripción del reto

RED

- Descripción del reto

    Un reto de análisis de imágenes o archivos con la pista de color "RED". Esto a menudo implica el análisis de canales de color en imágenes, esteganografía de color o el uso de una herramienta con el nombre del color.

- Procedimiento

    Identificación del problema: La bandera no se reveló con análisis forense básico.

    Herramientas usadas: zsteg (o análisis de canales RGB), GIMP (o Photoshop).

    Pasos para la solución:

        Descargué la imagen.

        Abrí la imagen en un editor de imágenes (como GIMP) y analicé los canales de color RGB individualmente, ocultando el rojo y el azul para ver el verde, etc.

        Alternativamente, usé zsteg o una herramienta similar para forzar la búsqueda en diferentes combinaciones de bits de color.

        Un canal de color o una capa de bits reveló un código oculto o la bandera.

- Solución

picoCTF{r3d_c4n_b3_h1dd3n_4c3d0b}

