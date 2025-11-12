### **vault-door-1**

#### **- Descripción del reto**
* El primer desafío de ingeniería inversa de código Java. La bandera es la contraseña que ha sido **mezclada o transpuesta** de una manera sencilla.

#### **- Procedimiento**
* **Identificación del problema:** La función `checkPassword` tomó la contraseña de 32 caracteres y la reordenó en bloques pequeños (ej., de 4 caracteres) antes de compararla.
* **Herramientas usadas:** Editor de texto, *script* de Python.
* **Pasos para la solución:**
  1.  Analicé la lógica de la función `checkPassword` y la cadena correcta de 32 caracteres.
  2.  Descubrí el **patrón de transposición** (ej., el byte 0 va a la posición 3, el byte 1 va a la posición 7, etc.).
  3.  Escribí un *script* simple en Python para tomar la cadena desordenada y aplicarle el patrón de reordenamiento inverso para obtener la contraseña original.
  4.  Introduje la contraseña reordenada en el programa.

#### **- Solución**
`picoCTF{v4ult_d00r_tr4nsp0s1t10n_34c2d1}`

---

