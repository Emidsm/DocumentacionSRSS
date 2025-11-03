basic-mod1

- Descripción del reto

    La bandera está cifrada utilizando operaciones matemáticas sencillas de módulo (mod), una técnica fundamental en la criptografía como la de César o RSA.

- Procedimiento

    Identificación del problema: Se proporcionó un código que cifraba el texto o una serie de números que requerían una operación módulo.

    Herramientas usadas: Python (para operaciones módulo), decodificador.

    Pasos para la solución:

        Analicé el script proporcionado y encontré la operación de cifrado (por ejemplo, c = (m + key) % 26).

        Identifiqué el valor clave (el offset o la clave).

        Escribí un script inverso para aplicar la operación de descifrado: m = (c - key) % 26.

        Apliqué la operación a la cadena cifrada para obtener la bandera.

- Solución

picoCTF{m0dul4r_4r1th_1s_34sy_f04e8a}

