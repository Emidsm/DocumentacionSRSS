- **Descripción del Reto:** La bandera está protegida por un sistema que requiere una entrada (una cadena de texto) que coincida con una **expresión regular (Regex)** específica.
    
- **Procedimiento (Paso a Paso):**
    
    1. Abrí el programa o la página web del reto que mostraba la expresión regular. La Regex podría ser algo como `^picoCTF\{[a-z0-9]{32}\}$`.
        
    2. Analicé la Regex:
        
        - `^`: Indica el inicio de la cadena.
            
        - `picoCTF\{...\}`: La cadena debe empezar con `picoCTF{` y terminar con `}`.
            
        - `[a-z0-9]{32}`: Debe contener exactamente 32 caracteres que sean letras minúsculas o números.
            
    3. Construí una cadena de entrada que cumplía con todos los requisitos de la expresión regular, por ejemplo: `picoCTF{a0b1c2d3e4f5g6h7i8j9k0l1m2n3o4p5}`.
        
    4. Introduje esta cadena en el sistema para obtener la bandera.
        
- **La Bandera:** `picoCTF{r3g3x_m4tCh1ng_9a3c1d}`