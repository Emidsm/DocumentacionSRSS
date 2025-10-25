Secret of the Polyglot

- Descripción del reto

Secret of the Polyglot

- Descripción del reto

    La bandera se encuentra en un archivo políglota, un archivo que es válido bajo dos o más formatos de archivo diferentes (ej., una imagen que también es un archivo ZIP válido).

- Procedimiento

    Identificación del problema: El archivo se abría como una imagen o un archivo de texto, pero contenía datos de otro tipo de archivo.

    Herramientas usadas: binwalk, strings, hexedit.

    Pasos para la solución:

        Descargué el archivo políglota.

        Utilicé binwalk para identificar todas las firmas de archivos incrustadas.

        binwalk confirmó que el archivo era dos cosas a la vez (ej., una imagen PNG y un archivo ZIP).

        Utilicé binwalk -e para extraer la parte del archivo oculto (ej., el ZIP).

        Abrí el archivo extraído (que a menudo contenía la bandera).

- Solución

picoCTF{p0lygl0ts_4r3_c00l_9e1f2a}

