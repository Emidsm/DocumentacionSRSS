- **Descripción del Reto:** La bandera está protegida por un sistema de autenticación basado en cookies. El objetivo es manipular el valor de una cookie para obtener acceso.
    
- **Procedimiento (Paso a Paso):**
    
    1. Abrí la página web y vi un mensaje que decía que solo el usuario "admin" podía acceder.
        
    2. Usé la herramienta de desarrollo del navegador para inspeccionar las cookies.
        
    3. Encontré una cookie llamada `is_admin` con el valor `False`.
        
    4. Cambié el valor de esa cookie de `False` a `True` y recargué la página.
        
    5. Al hacerlo, el sitio me reconoció como administrador y me mostró la bandera.
        
- **La Bandera:** `picoCTF{n0t_4_r34l_4dm1n_488950}`