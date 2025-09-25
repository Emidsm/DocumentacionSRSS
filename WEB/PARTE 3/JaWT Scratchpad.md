- **Descripción del Reto:** La bandera está protegida por un token web JSON (JWT). El objetivo es manipular el token JWT para obtener acceso de administrador y conseguir la bandera.
    
- **Procedimiento (Paso a Paso):**
    
    1. Abrí la página web y me registré. Al hacerlo, el servidor me dio un token JWT.
        
    2. Usé una herramienta en línea o un decodificador de JWT para analizar el token.
        
    3. El token tenía un campo de "username" con mi nombre de usuario y un campo de "admin" con el valor `false`.
        
    4. Cambié el valor del campo "admin" a `true`, pero el token no era válido debido a la firma.
        
    5. Descubrí que la firma se generaba con una clave secreta. El reto me dio una pista para cambiar el algoritmo de firma a `None`.
        
    6. Modifiqué el campo "alg" de la cabecera a `none` y eliminé la firma del token.
        
    7. Envié el token modificado al servidor en una nueva solicitud. El servidor me reconoció como administrador y me dio la bandera.
        
- **La Bandera:** `picoCTF{n0t_s0_s3cur3_JWt_d3118d}`