### **Picker II**

#### **- Descripción del reto**
* Desafío de explotación que requiere manipular la **lógica de selección** y sobrescribir un puntero de función para forzar el salto a la función de la bandera.

#### **- Procedimiento**
* **Identificación del problema:** El reto implicaba un *exploit* que manipulaba punteros en la pila o en el área de datos.
* **Herramientas usadas:** Desensamblador, *script* de Python (`pwntools`).
* **Pasos para la solución:**
  1.  Analicé cómo se indexaban las opciones y cómo se almacenaban los punteros a las funciones.
  2.  Exploré una vulnerabilidad que permitía **sobrescribir un puntero de función** con la dirección de la función `win_function` (o la función que imprime la bandera).
  3.  Forcé al programa a ejecutar la función comprometida para obtener la bandera.

#### **- Solución**
`picoCTF{p1ck3r_ii_m0r3_fun_a5d4c1}`

