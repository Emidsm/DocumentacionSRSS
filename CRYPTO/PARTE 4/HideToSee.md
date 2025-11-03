HideToSee

- Descripción del reto

    La bandera está oculta en un archivo de imagen o un documento que utiliza esteganografía de datos nulos o una simple manipulación de metadatos.

- Procedimiento

    Identificación del problema: La bandera no era visible a simple vista y requería una inspección del contenido binario.

    Herramientas usadas: strings, exiftool.

    Pasos para la solución:

        Descargué el archivo de imagen.

        Utilicé el comando strings en el archivo para extraer todo el texto legible. El comando fue strings [nombre_de_archivo] | grep picoCTF.

        La bandera estaba oculta al final del archivo, más allá de la información de la imagen, y se reveló en la salida de strings.

- Solución

picoCTF{h1d3_th3_d4t4_b3h1nd_7h3_d0ts_f5d1a2}

