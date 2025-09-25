- **Descripción del Reto:** Este es un desafío de inyección SQL más avanzado que el anterior, donde el objetivo es no solo autenticarse, sino también extraer información de otras tablas de la base de datos.
    
- **Procedimiento (Paso a Paso):**
    
    1. Usé una técnica de **inyección de unión** (UNION injection) para combinar mi consulta con otra consulta que extrajera información de una tabla del sistema.
        
    2. En el campo de "username", ingresé `' UNION SELECT username, password FROM users --`.
        
    3. El servidor me mostró la bandera en la columna de la contraseña.
        
    4. También pude usar inyección de unión para obtener el nombre de las tablas y las columnas de la base de datos para extraer la bandera de una tabla no estándar.
        
- **La Bandera:** `picoCTF{m0r3_sQl_1nj3ct10n_b867c4}`