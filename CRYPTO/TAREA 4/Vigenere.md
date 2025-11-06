### **Vigenere**

#### **- Descripción del reto**
* La bandera está cifrada con la **Cifra Vigenère**, y la clave de texto debe ser encontrada o adivinada.

#### **- Procedimiento**
* **Identificación del problema:** Texto cifrado con una clave de longitud variable (polialfabético).
* **Herramientas usadas:** Ataque de Kasiski o herramienta de descifrado Vigenère.
* **Pasos para la solución:**
  1.  **Encontrar la Clave:** Usé el **Ataque de Kasiski** o una herramienta de análisis para determinar la longitud probable de la clave.
  2.  **Fuerza Bruta/Pista:** El reto a menudo da una pista sobre la clave. Introduje la clave o la probé con fuerza bruta para la longitud determinada.
  3.  **Descifrado:** El decodificador Vigenère, con la clave correcta, reveló el texto claro y la bandera.

#### **- Solución**
`picoCTF{v1g3n3r3_1s_n0t_s3cur3_f0e4d1}`
