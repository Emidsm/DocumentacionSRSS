#### **- Descripción del reto**

- La bandera está cifrada con la Cifra César, pero el desplazamiento (la clave) es desconocido y debe ser determinado por fuerza bruta o análisis.
    

#### **- Procedimiento**

- **Identificación del problema:** La bandera estaba cifrada con un desplazamiento desconocido de la Cifra César.
    
- **Herramientas usadas:** Script de fuerza bruta para Cifra César.
    
- **Pasos para la solución:**
    
    1. Tomé la cadena cifrada.
        
    2. Apliqué fuerza bruta a todos los posibles desplazamientos (1 a 25).
        
    3. Identifiqué el desplazamiento que resultó en texto legible (ej., el prefijo "picoCTF").
        
    4. Utilicé ese desplazamiento para decodificar la cadena completa y obtener la bandera.
        

#### **- Solución**

`picoCTF{c43s4r_c1ph3r_4n4lys1s_f8e4c1}`

---

