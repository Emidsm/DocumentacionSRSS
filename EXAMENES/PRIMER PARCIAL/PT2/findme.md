- **Descripción del Reto:** La bandera está oculta dentro del _script_ o binario de un programa, y el reto consiste en encontrar el código o _string_ que contiene el valor de la bandera.
    
- **Procedimiento (Paso a Paso):**
    
    1. Descargué el archivo ejecutable (`findme`).
        
    2. Utilicé el comando **`strings`** en el binario para extraer todas las cadenas de texto legible.
        
    3. Filté la salida del comando `strings` usando `grep picoCTF` para buscar directamente la bandera.
        
    4. El comando final fue `strings findme | grep picoCTF`.
        
    5. Encontré la bandera codificada o sin codificar en la salida del _grep_.
        
- La Bandera:
    
    picoCTF{f1nd1ng_th3_s7r1ngs_4r3_3z_b0c1f2}