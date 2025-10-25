
information

- Descripción del reto

    La bandera está oculta en los metadatos de un archivo (a menudo una imagen) o dentro del archivo mismo, requiriendo un análisis forense simple.

- Procedimiento

    Identificación del problema: Se proporcionó un archivo que no contenía la bandera visiblemente.

    Herramientas usadas: exiftool, strings.

    Pasos para la solución:

        Descargué el archivo proporcionado.

        Utilicé la herramienta exiftool para extraer todos los metadatos de la imagen.

        Revisé los campos comunes de metadatos (Autor, Comentarios, Derechos de Autor, etc.).

        Encontré la bandera o una pista en uno de los campos de metadatos.

- Solución

picoCTF{m3t4d4t4_n3v3r_l13s_14c330}

