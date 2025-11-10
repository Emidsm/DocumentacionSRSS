### **vault-door-4**

#### **- Descripción del reto**
* La bandera está cifrada utilizando la Cifra **Base64** en el código Java. El reto es identificar la codificación y revertirla.

#### **- Procedimiento**
* **Identificación del problema:** El código Java hizo referencia a la librería `java.util.Base64` o aplicó un patrón reconocible de Base64 al *string* de la contraseña.
* **Herramientas usadas:** Editor de texto, decodificador Base64 en línea.
* **Pasos para la solución:**
  1.  Identifiqué el *string* cifrado dentro de la función `checkPassword`.
  2.  Noté que el *string* estaba siendo manipulado antes de ser comparado, y la manipulación se ajustaba al patrón de codificación **Base64**.
  3.  Copié la cadena y la decodifiqué utilizando una herramienta de decodificación Base64 en línea.
  4.  La cadena decodificada fue la contraseña.

#### **- Solución**
`picoCTF{b4s3d_0n_wh4t_1_s33_54d1c2}`

---

