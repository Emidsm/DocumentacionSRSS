hideme

- Descripción del reto

hideme

- Descripción del reto

    La bandera está oculta en un archivo (a menudo una imagen) que contiene otra información incrustada o archivos anidados.

- Procedimiento

    Identificación del problema: El archivo contenía datos adicionales que no pertenecían a su formato.

    Herramientas usadas: binwalk, strings.

    Pasos para la solución:

        Descargué el archivo.

        Utilicé la herramienta binwalk para escanear el archivo en busca de firmas de archivos incrustados (ej., zip, jpeg, png). El comando fue binwalk [nombre_de_archivo].

        binwalk identificó un archivo comprimido (.zip o .tar) incrustado.

        Utilicé binwalk -e [nombre_de_archivo] para extraer los archivos ocultos y encontré la bandera.

- Solución

picoCTF{h1dd3n_d4t4_r3tr13v3d_8e4c1f}

