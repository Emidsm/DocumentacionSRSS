St3g0

- Descripción del reto

St3g0

- Descripción del reto

    La bandera está oculta utilizando esteganografía simple en una imagen, a menudo en los bits menos significativos (LSB) o metadatos.

- Procedimiento

    Identificación del problema: La bandera no estaba en los metadatos, por lo que se requería una técnica de esteganografía.

    Herramientas usadas: zsteg, steghide (o análisis LSB).

    Pasos para la solución:

        Descargué la imagen.

        Utilicé la herramienta zsteg para automatizar la búsqueda de datos ocultos en los bits de la imagen. El comando fue zsteg [nombre_de_archivo].

        zsteg reportó una cadena de texto (a veces codificada en Base64) incrustada.

        Decodifiqué la cadena para obtener la bandera.

- Solución

picoCTF{st3g0_1s_n0t_h4rd_92f587}

