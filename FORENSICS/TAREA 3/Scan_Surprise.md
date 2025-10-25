Scan Surprise

- Descripción del reto

Scan Surprise

- Descripción del reto

    El desafío se enfoca en el análisis de un programa binario que realiza una operación de escaneo de la entrada, siendo vulnerable a una condición de buffer overflow o un format string simple.

- Procedimiento

    Identificación del problema: El programa utiliza la función scanf() o un equivalente de manera insegura.

    Herramientas usadas: gdb (o un depurador), format string payload.

    Pasos para la solución:

        Ejecuté el programa y analicé su comportamiento.

        Descubrí que la función de escaneo no validaba la longitud de la entrada.

        Envié un payload de format string (como %x repetido) para volcar la pila y buscar una dirección que contenía la bandera.

        El format string reveló la dirección de memoria donde se almacenaba el string de la bandera.

- Solución

picoCTF{sc4n_surpr1se_g0t_y0u_d11a2c}

