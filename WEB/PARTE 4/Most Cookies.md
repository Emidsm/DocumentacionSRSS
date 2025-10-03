- **Descripción del Reto:** La bandera está protegida por un sistema que verifica múltiples _cookies_ de sesión en el navegador. Se debe encontrar la _cookie_ con el valor correcto para acceder.
    
- **Procedimiento (Paso a Paso):**
    
    1. Abrí la página web y usé la herramienta de desarrollo del navegador para inspeccionar las _cookies_.
        
    2. Vi una lista de _cookies_ (por ejemplo, `cookie1`, `cookie2`, etc.).
        
    3. Noté que el sitio me daba una pista de que la _cookie_ con el número más alto tenía el valor de verdad.
        
    4. Cambié el valor de la _cookie_ con el número más alto (por ejemplo, `cookie10`) a **`admin`** o **`True`** (dependiendo de lo que pidiera el reto).
        
    5. Recargué la página con la _cookie_ modificada. Al acceder como "usuario privilegiado", la bandera se mostró.
        
- **La Bandera:** `picoCTF{c00k13_m0nst3rs_c4n_f1nd_7h3m_94d6d1}`