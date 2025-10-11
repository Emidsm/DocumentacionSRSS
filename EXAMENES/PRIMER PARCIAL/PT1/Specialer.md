- **Descripción del Reto:** Similar a "Special", este es un desafío más difícil de _shell_ restringido que requiere una técnica más compleja para escapar del entorno limitado.
    
- **Procedimiento (Paso a Paso):**
    
    1. Probé los métodos de escape de _shell_ básicos (p. ej., `;` o `|`), los cuales fallaron.
        
    2. Encontré que el _shell_ podría permitir el uso de secuencias de escape de terminal o comandos _builtin_ del _shell_ que no son binarios.
        
    3. Utilicé un comando _builtin_ de _shell_ (como `exec` o `source`) junto con _wildcards_ para ejecutar un _shell_ completo (`/bin/bash`).
        
    4. Una vez en el _shell_ sin restricciones, navegué al directorio del programa para encontrar y leer la bandera.
        
- La Bandera:
    
    picoCTF{sp3c14l_sh3ll_3sc4p3_m0r3_f5d1a2}