#### **- Descripción del reto**

- La bandera se obtiene a través de la explotación de una función de servidor sin estado (**Serverless/Lambda**) que es vulnerable a la inyección de código o comandos.
    

#### **- Procedimiento**

- **Identificación del problema:** El servidor sin estado procesa la entrada del usuario directamente, lo que sugiere una vulnerabilidad de inyección de comandos OS.
    
- **Herramientas usadas:** Navegador, inyección de comandos OS.
    
- **Pasos para la solución:**
    
    1. Probé el _endpoint_ de Lambda con una inyección simple para ver si ejecutaba código.
        
    2. Utilicé un _payload_ de inyección de comandos OS (ej., `& ls &`) para listar los archivos.
        
    3. Encontré el archivo de la bandera (ej., `flag.txt`) y usé el comando `cat` para leerlo a través de la inyección (`& cat flag.txt &`).
        

#### **- Solución**

`picoCTF{l4mbd4_1nj3ct10n_fTw_e2c1b2}`

---

