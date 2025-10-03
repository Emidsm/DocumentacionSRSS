- **Descripción del Reto:** Este desafío se enfoca en la **criptografía** o codificación de datos. El nombre "Trickster" (Bromista/Tramposo) sugiere que la codificación utilizada no es obvia o es una que se usa comúnmente para ofuscar información (como ROT13, Base64 o una cifra simple).
    
- **Procedimiento (Paso a Paso):**
    
    1. Recibí una cadena de texto codificada o cifrada.
        
    2. Analicé la cadena en busca de patrones. Si contenía solo letras y números, sospeché de Base64. Si solo contenía letras, pensé en ROT13 o la Cifra César.
        
    3. Identifiqué que era una **Cifra César** (o ROT _n_) debido a la presencia de letras.
        
    4. Usé una herramienta de descifrado en línea o un _script_ simple para probar diferentes _offsets_ de la cifra César hasta que el texto se volvió legible y reveló la bandera.
        
- **La Bandera:** `picoCTF{tr1ckst3r_c1ph3r_r3v34l3d_94d6e1}`
    
