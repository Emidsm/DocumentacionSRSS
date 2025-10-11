- **Descripción del Reto:** La bandera está protegida por una restricción de entrada que prohíbe el uso de caracteres alfabéticos (a-z, A-Z). Debo inyectar código utilizando solo caracteres no alfabéticos.
    
- **Procedimiento (Paso a Paso):**
    
    1. El programa solo aceptaba números y símbolos.
        
    2. Utilicé una técnica de **codificación _sans-alpha_** (sin alfabeto), que a menudo implica la construcción de comandos a través de operaciones XOR o _bitwise_ con cadenas de símbolos.
        
    3. Construí el _payload_ para ejecutar el comando `/bin/sh` y luego `ls` para encontrar la bandera.
        
    4. Ejecuté el _payload_ para obtener acceso al _shell_ y leer el archivo de la bandera.
        
- La Bandera:
    
    picoCTF{s4ns_4lph4_g3n3r4t0r_1s_k3y_94d6e1}