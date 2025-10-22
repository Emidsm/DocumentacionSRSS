### ****

- **Descripción del Reto:** La bandera se obtiene al utilizar la herramienta de _proxy_ **Burp Suite** para interceptar y modificar una solicitud HTTP.
    
- **Procedimiento (Paso a Paso):**
    
    1. Configuré mi navegador para usar **Burp Suite** como _proxy_ HTTP.
        
    2. Activé la función "Intercept is on" en Burp Suite y cargué la página web.
        
    3. La solicitud HTTP quedó en espera en Burp Suite.
        
    4. Analicé las cabeceras y el cuerpo de la solicitud. Encontré una cabecera o un parámetro que debía ser modificado (por ejemplo, `role: guest` a `role: admin`).
        
    5. Modifiqué el valor, reenvié la solicitud y la respuesta del servidor contenía la bandera.
        
- La Bandera:
    
    picoCTF{burp_1s_b3tter_th4n_z4p_8e4c1f}