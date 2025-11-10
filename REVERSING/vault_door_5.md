### **vault-door-5**

#### **- Descripción del reto**
* La bandera está cifrada con una **combinación de algoritmos** y *offsets*, lo que requiere ingeniería inversa de múltiples pasos.

#### **- Procedimiento**
* **Identificación del problema:** La función `checkPassword` aplicó una mezcla de **transposición** (como en `vault-door-1`) y alguna forma de **cifrado Vigenère** o **sustitución** (como `vault-door-4`).
* **Herramientas usadas:** Editor de texto, *script* de Python.
* **Pasos para la solución:**
  1.  **Paso 1: Separación de algoritmos:** Dividí el código en secciones, identificando el cifrado de transposición y el cifrado de sustitución.
  2.  **Paso 2: Reversión del Cifrado de Sustitución:** Revertí la parte más fácil (ej., Base64 o ROT).
  3.  **Paso 3: Reversión de la Transposición:** Apliqué el patrón de reordenamiento inverso a los bloques de caracteres de la cadena resultante.
  4.  El resultado final fue la contraseña de texto claro.

#### **- Solución**
`picoCTF{m1x3d_4nd_m4tch3d_c1ph3r5_93e2a1}`
