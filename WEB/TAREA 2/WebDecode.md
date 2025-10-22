- **Descripción del Reto:** La bandera está codificada con una técnica de codificación web común (como URL encoding o Base64) y debe ser decodificada para revelarla.
    
- **Procedimiento (Paso a Paso):**
    
    1. Recibí una cadena de texto larga que contenía muchos `%` o terminaba con un `=` o `==`.
        
    2. Si contenía `%` y caracteres hexadecimales (ej. `%20`), apliqué **URL Decoding**.
        
    3. Si terminaba con `=` o `==` y contenía letras, números y `+` o `/`, apliqué **Base64 Decoding**.
        
    4. El proceso de decodificación (a veces en múltiples capas) reveló la bandera.
        
- La Bandera:
    
    picoCTF{d3c0d3_w3b_d4t4_50d1a2}