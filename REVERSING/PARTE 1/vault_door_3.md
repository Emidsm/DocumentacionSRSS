### **vault-door-3**

#### **- Descripción del reto**
* La bandera está cifrada utilizando una combinación de **rotaciones bit a bit** y **operaciones XOR** en el código Java.

#### **- Procedimiento**
* **Identificación del problema:** La función `checkPassword` aplicó múltiples capas de manipulación bit a bit a la contraseña de entrada.
* **Herramientas usadas:** Editor de texto, *script* de Python (para operaciones bit a bit).
* **Pasos para la solución:**
  1.  Analicé el código Java, identificando las operaciones como `c = (b >> 4) | (b << 4)` (rotación de 4 bits) y `c = b ^ 0x55` (XOR con un valor constante).
  2.  Escribí un *script* de Python para realizar la **operación inversa** a cada byte de la cadena cifrada. La operación inversa de `(b >> 4) | (b << 4)` es la misma operación, y la inversa de XOR es la misma XOR.
  3.  Apliqué las operaciones inversas en el orden inverso al que se aplicaron en la función.
  4.  El resultado fue la contraseña de texto claro.

#### **- Solución**
`picoCTF{r0t4t1ng_4nd_x0r1ng_1s_fun_8e4c1f}`

---

