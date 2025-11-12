### **Safe Opener**

#### **- Descripción del reto**
* El reto consiste en encontrar la clave de una "caja fuerte" protegida por un programa binario. La clave está **hardcodeada** o codificada de manera simple en el ejecutable.

#### **- Procedimiento**
* **Identificación del problema:** La contraseña es estática y debe ser extraída del binario sin ejecutar el programa.
* **Herramientas usadas:** `strings`, `gdb` (para inspección estática).
* **Pasos para la solución:**
  1.  Utilicé el comando **`strings`** en el binario para volcar todas las cadenas de texto legible.
  2.  Filté la salida buscando cadenas que parecieran contraseñas o que se compararan con la entrada del usuario.
  3.  Encontré la contraseña correcta *hardcodeada* cerca de la función de comparación de *strings*.
  4.  Ejecuté el programa e introduje la contraseña para obtener la bandera.

#### **- Solución**
`picoCTF{s4f3_0p3n3r_g0t_th3_c0d3_94d6e1}`

