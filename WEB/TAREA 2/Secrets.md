- **Descripción del Reto:** La bandera está oculta en un archivo de configuración, _logs_ o un directorio sensible que el servidor expone accidentalmente.
    
- **Procedimiento (Paso a Paso):**
    
    1. Revisé el código fuente en busca de pistas sobre el _backend_ (por ejemplo, PHP, Python).
        
    2. Intenté acceder a rutas comunes donde los desarrolladores olvidan secretos: `.git`, `.env`, `config.php`, o `backup.zip`.
        
    3. El código fuente de la página dio una pista sobre un archivo `.git/config` o un directorio expuesto.
        
    4. Navegué a la ruta del archivo de configuración sensible y leí su contenido, donde estaba la bandera.
        
- La Bandera:
    
    picoCTF{s3cr3t5_d0n7_g0_1n_th3_fr0nt3nd_8e4c1f}
