Redaction gone wrong

- Descripción del reto

Redaction gone wrong

- Descripción del reto

    La bandera fue "tachada" o redactada en un documento PDF, pero no eliminada del archivo subyacente.

- Procedimiento

    Identificación del problema: El documento PDF mostraba texto importante cubierto por barras negras o cuadros de colores.

    Herramientas usadas: Editor de texto simple, visor de PDF avanzado, o herramientas de línea de comandos.

    Pasos para la solución:

        Abrí el archivo PDF con un editor de texto simple (o un visor de PDF que permite copiar el texto subyacente).

        Al copiar el texto, el texto redactado se reveló.

        Alternativamente, analicé el contenido XML o stream del PDF (descomprimiéndolo) y encontré la cadena de texto no visible.

- Solución

picoCTF{r3d4ct10n_1s_n0t_d3l3t10n_f3a1d9}

