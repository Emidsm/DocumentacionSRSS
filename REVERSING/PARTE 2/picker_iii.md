### **Picker III**

#### **- Descripción del reto**
* Un desafío de explotación binaria que requiere el uso de un **ataque de *format string*** para obtener el control del flujo del programa o leer/escribir memoria arbitraria.

#### **- Procedimiento**
* **Identificación del problema:** El programa utilizaba una función insegura (ej., `printf(input)`) que permitía la inyección de especificadores de formato.
* **Herramientas usadas:** *Script* de Python (`pwntools`), `gdb`.
* **Pasos para la solución:**
  1.  Identifiqué la vulnerabilidad de **`format string`**.
  2.  Usé especificadores de formato (ej., `%x`, `%p`) para **filtrar direcciones de memoria** importantes.
  3.  Usé el *format string* para **escribir** una nueva dirección en la pila, sobrescribiendo el puntero de la Dirección de Retorno (RIP/EIP) para saltar a la función de la bandera.

#### **- Solución**
`picoCTF{p1ck3r_iii_st4ck_sm4sh_e2c1b2}`

