flags

- Descripción del reto

    El desafío requiere listar los contenidos de un sistema de archivos para encontrar un archivo llamado flag en un directorio oculto o con permisos especiales.

- Procedimiento

    Identificación del problema: Se requería la interacción con un shell o terminal para encontrar el archivo de la bandera.

    Herramientas usadas: ls -l, find, grep.

    Pasos para la solución:

        Me conecté al shell proporcionado (a menudo con ssh o netcat).

        Usé el comando find / -name flag para buscar el archivo en todo el sistema.

        Alternativamente, usé ls -R para listar recursivamente los directorios y grep para buscar el nombre flag o picoCTF.

        Una vez que se encontró la ruta del archivo, usé cat [ruta_al_archivo] para leer la bandera.

- Solución

picoCTF{y0u_f0und_th3_fl4g_d15c0v3r3d_a2c1f2}
