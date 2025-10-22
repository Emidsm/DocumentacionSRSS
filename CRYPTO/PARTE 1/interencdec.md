#### **- Descripción del reto**

- La bandera ha sido cifrada o codificada **múltiples veces (intercaladas)** con diferentes métodos (ej. Base64, Hexadecimal, URL Encoding).
    

#### **- Procedimiento**

- **Identificación del problema:** La cadena resultante parecía ilegible y la decodificación simple no funcionó, mostrando patrones de múltiples codificaciones.
    
- **Herramientas usadas:** Herramientas de decodificación en línea.
    
- **Pasos para la solución:**
    
    1. Identifiqué la codificación más externa (ej., URL encoding) y decodifiqué esa capa.
        
    2. El resultado reveló una nueva capa de codificación (ej., Hexadecimal).
        
    3. Repetí el proceso de decodificación e identificación hasta que se reveló el prefijo legible "picoCTF".
        

#### **- Solución**

`picoCTF{m4ny_l4y3r5_0f_c0d1ng_a9b31d}`