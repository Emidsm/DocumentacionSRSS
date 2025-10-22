- **Descripción del Reto:** Un reto de **Inyección SQL** que se enfoca en la sintaxis específica de la base de datos **SQLite**, que a menudo se usa en desafíos sencillos.
    
- **Procedimiento (Paso a Paso):**
    
    1. Identifiqué el formulario de _login_ vulnerable.
        
    2. Utilicé la inyección de _bypass_ de _login_ básica para SQLite, que a menudo es `' OR 1=1 --`.
        
    3. La inyección exitosa me autenticó como el primer usuario (generalmente el administrador), lo que me dio acceso a la bandera.
        
- La Bandera:
    
    picoCTF{sq11t3_1nj3ct10n_f0r_th3_w1n_e2c1b2}