### **Safe Opener 2**

#### **- Descripción del reto**
* Una versión avanzada de Safe Opener, donde la clave no está *hardcodeada* sino que se **genera dinámicamente** mediante una función de transformación matemática dentro del programa.

#### **- Procedimiento**
* **Identificación del problema:** La contraseña es el resultado de aplicar una función inversa a un *string* cifrado que está en el código.
* **Herramientas usadas:** Desensamblador (como **Ghidra** o **IDA Pro**), *script* de Python.
* **Pasos para la solución:**
  1.  Abrí el binario en un desensamblador y analicé la función que comprueba la contraseña.
  2.  Identifiqué la **lógica de generación** (ej., XOR con un valor constante, suma de *offsets*, o rotación de *bits*).
  3.  Escribí un *script* simple en Python para **revertir la lógica** de la función y calcular la entrada correcta.
  4.  Introduje el valor calculado en el programa para obtener la bandera.

#### **- Solución**
`picoCTF{s4f3_0p3n3r_c0d3_g3n3r4t0r_3f2b45}`

