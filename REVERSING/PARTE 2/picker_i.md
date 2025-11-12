### **Picker I**

#### **- Descripción del reto**
* Primer desafío de la serie Picker. Explotación de un programa de menú que permite **sobrescribir una variable booleana simple** (ej., `is_admin`) a través de un *exploit* de índice o *buffer* simple.

#### **- Procedimiento**
* **Identificación del problema:** El programa permitía al usuario manipular variables internas, como un *flag* de administración, debido a una validación de índice deficiente.
* **Herramientas usadas:** Desensamblador, *script* de Python.
* **Pasos para la solución:**
  1.  Identifiqué una opción que permitía la **escritura fuera de límites** de un array de opciones.
  2.  Calculé el *offset* de la variable `is_admin` con respecto al array.
  3.  Utilicé la opción de escritura para cambiar el valor de `is_admin` de `0` a `1` y obtener acceso a la función de la bandera.

#### **- Solución**
`picoCTF{p1ck3r_i_s0_s1mpl3_f48d91}`

