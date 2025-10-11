- **Descripción del Reto:** La bandera está protegida por un sistema de _login_ que requiere una contraseña cuyo _hash_ coincida con un valor precalculado. El reto implica encontrar la cadena original a partir de su _hash_.
    
- **Procedimiento (Paso a Paso):**
    
    1. El _script_ del programa mostró el valor de _hash_ esperado y el algoritmo utilizado (por ejemplo, SHA-256).
        
    2. Analicé las pistas sobre la contraseña (a menudo es una palabra común, una _leet speak_ o una secuencia simple de caracteres).
        
    3. Utilicé un sitio web de _hash lookup_ (búsqueda de _hash_ en bases de datos) o una herramienta como **`hashcat`** para intentar hacer _cracking_ de _hash_.
        
    4. Una vez que se encontró la contraseña original, la introduje en el programa para obtener la bandera.
        
- La Bandera:
    
    picoCTF{h4sh1ng_1s_n0t_3ncrypt10n_a0c1b2}
    
