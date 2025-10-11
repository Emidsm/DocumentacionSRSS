- **Descripción del Reto:** Este es un desafío de **inyección SQL** donde la interacción se realiza directamente a través de un _endpoint_ o un programa, no solo a través de un formulario de _login_.
    
- **Procedimiento (Paso a Paso):**
    
    1. Identifiqué el parámetro vulnerable en la URL o en la línea de comandos.
        
    2. Utilicé la inyección de unión (`UNION SELECT`) para enumerar la información de la base de datos.
        
    3. **Paso de Enumeración (Ejemplo):**
        
        - Determiné el número de columnas (`' ORDER BY N --`).
            
        - Encontré las columnas visibles (`' UNION SELECT 1, 2, 'abc' --`).
            
        - Obtuve el nombre de la tabla de _users_ (`' UNION SELECT table_name, 2, 3 FROM information_schema.tables WHERE table_schema = database() --`).
            
    4. Una vez que la tabla de la bandera fue identificada, extraje su contenido: `' UNION SELECT flag, 2, 3 FROM flag_table --`.
        
- La Bandera:
    
    picoCTF{sq1_d1r3c7_4cc3ss_74d9e1}