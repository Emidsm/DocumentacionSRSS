- **Descripción del Reto:** La bandera está protegida por un sistema de _cookies_, pero en lugar de solo cambiar un valor, la _cookie_ está firmada o codificada, y la clave secreta se revela en un punto.
    
- **Procedimiento (Paso a Paso):**
    
    1. Revisé la _cookie_ de sesión y noté que estaba codificada (a menudo Base64).
        
    2. Decodifiqué la _cookie_ y vi que contenía datos como `{"user": "guest"}`.
        
    3. El reto proporcionó una pista, a menudo en el _source_ de la página o en un archivo adicional, que revelaba la **clave secreta** utilizada para firmar la _cookie_.
        
    4. Utilicé la clave secreta para regenerar una _cookie_ modificada (`{"user": "admin"}`) y la volví a firmar con un _script_ simple.
        
    5. Sustituí la _cookie_ en mi navegador por la nueva _cookie_ de administrador para obtener la bandera.
        
- La Bandera:
    
    picoCTF{c00k1e_m0nst3r_s3cr3t_r3c1p3_a5d4c1}
