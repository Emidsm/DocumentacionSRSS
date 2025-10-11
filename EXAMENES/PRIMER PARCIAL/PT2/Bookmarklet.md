- **Descripción del Reto:** La bandera está oculta en un entorno web que permite la ejecución de código JavaScript malicioso a través de una **Bookmarklet** (un _bookmark_ que ejecuta código).
    
- **Procedimiento (Paso a Paso):**
    
    1. El reto proporcionaba un mecanismo para crear o usar _bookmarklets_.
        
    2. El objetivo era inyectar código JavaScript que ejecutara una acción en la página o que intentara robar información (como _cookies_ o el _source_ de la página).
        
    3. Construí una _bookmarklet_ simple, como `javascript:alert(document.domain)` para confirmar la inyección.
        
    4. Luego, modifiqué la _bookmarklet_ para obtener el contenido del _source_ de la página o para acceder a una variable global que contenía la bandera, a menudo usando `javascript:fetch('/flag').then(r=>r.text()).then(t=>alert(t))` o un código similar.
        
- La Bandera:
    
    picoCTF{b00km4rk1ng_1s_fun_f48d91}