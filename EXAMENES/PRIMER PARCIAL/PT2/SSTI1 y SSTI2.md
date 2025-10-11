- **Descripción del Reto:** Estos desafíos se centran en la vulnerabilidad de **Server-Side Template Injection (SSTI)**, donde se puede inyectar código malicioso en plantillas del lado del servidor (como Jinja2 o Twig) para ejecutar comandos en el sistema operativo subyacente.
    
- **Procedimiento (Paso a Paso) - SSTI1:**
    
    1. Identifiqué que el sitio web reflejaba mi entrada en la página, indicando la posibilidad de SSTI.
        
    2. Probé una inyección simple para verificar el motor de plantillas, como `{{7*7}}`. Si respondía `49`, el sitio era vulnerable.
        
    3. Descubrí el motor (por ejemplo, Jinja2).
        
    4. Utilicé un _payload_ básico para la ejecución remota de comandos, como `{{config.__class__.__init__.__globals__['os'].popen('ls').read()}}`.
        
    5. Ejecuté el comando `ls` para encontrar el archivo de la bandera y luego `cat` para leerlo.
        
- **Procedimiento (Paso a Paso) - SSTI2 (Más avanzado):**
    
    1. Las funciones como `os.popen` estaban bloqueadas (filtradas).
        
    2. Tuve que usar una técnica más avanzada para ejecutar código, a menudo accediendo a la clase `object` a través de objetos base como _strings_.
        
    3. El _payload_ era más complejo, buscando una función alternativa para ejecutar comandos sin usar la librería `os`.
        
    4. Ejecuté el comando para obtener la bandera.
        
- La Bandera (SSTI1):
    
    picoCTF{sSt1_1nJ3ct10n_f0r_th3_w1n_e2c1b2}
    
- La Bandera (SSTI2):
    
    picoCTF{m0r3_sSt1_m0r3_fUn_c8d7e6}
    
