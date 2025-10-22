
- **Descripción del Reto:** La bandera está protegida por un valor de _cookie_ codificado o cifrado que debe ser modificado a un estado de "administrador" para obtener acceso.
    
- **Procedimiento (Paso a Paso):**
    
    1. Inspeccioné las _cookies_ del navegador. Encontré una _cookie_ con un valor largo, probablemente codificado en **Base64**.
        
    2. Decodifiqué el valor Base64, que reveló una cadena JSON o un _string_ de texto simple (ej. `user=guest`).
        
    3. Modifiqué el valor decodificado a `user=admin`.
        
    4. Volví a codificar el _string_ modificado a Base64.
        
    5. Sustituí la _cookie_ original por el nuevo valor codificado y recargué la página para obtener la bandera.
        
- La Bandera:
    
    picoCTF{p0w3r_c00k13_m4n1pul4t10n_94d6e1}
    

---
