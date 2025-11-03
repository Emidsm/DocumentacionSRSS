ReadMyCert

- Descripción del reto

    La bandera está oculta en el contenido de un certificado digital (X.509), que puede ser un archivo .pem, .crt, o similar.

- Procedimiento

    Identificación del problema: Se proporcionó un archivo de certificado digital.

    Herramientas usadas: openssl, visor de certificados.

    Pasos para la solución:

        Utilicé el comando openssl para analizar el contenido del certificado y mostrar los campos de texto. El comando fue openssl x509 -in [archivo.pem] -text -noout.

        Revisé la salida del comando. La bandera estaba a menudo oculta en un campo poco común como Organizational Unit (OU), Comments, o en la sección de Extensiones.

        Copié la bandera de la salida del texto.

- Solución

picoCTF{c3rt1f1c4t3s_4r3_r34d4b13_94d6e1}

