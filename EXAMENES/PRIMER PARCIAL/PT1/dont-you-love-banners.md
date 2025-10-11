- **Descripción del Reto:** La bandera está oculta en los datos que se obtienen después de una interacción sencilla con un puerto de red (un _banner_).
    
- **Procedimiento (Paso a Paso):**
    
    1. El reto proporcionó una dirección IP y un número de puerto.
        
    2. Utilicé el cliente **`netcat`** (`nc`) para conectarme al puerto: `nc [IP] [puerto]`.
        
    3. Al conectarme, el servidor inmediatamente envió un "banner" (un mensaje de bienvenida) que contenía la bandera.
        
- La Bandera:
    
    picoCTF{b4nn3r5_4r3_fun_50d1a2}
    
