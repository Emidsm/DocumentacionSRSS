### **Crack the Power**

#### **- Descripción del reto**
* La bandera está protegida por una contraseña, y se proporciona un archivo de *hash* simple. El reto consiste en realizar un **ataque de diccionario** o **fuerza bruta** para encontrar la contraseña.

#### **- Procedimiento**
* **Identificación del problema:** Se proporcionó un archivo de *hash* (a menudo MD5 o SHA1 simple) que debía ser craqueado.
* **Herramientas usadas:** Herramientas de *cracking* de contraseñas (ej., **Hashcat** o **John the Ripper**).
* **Pasos para la solución:**
  1.  Identifiqué el algoritmo de *hashing* utilizado.
  2.  Utilicé John the Ripper (con una lista de palabras común como `rockyou.txt`) o Hashcat para intentar descifrar el *hash*.
  3.  El *cracker* encontró la contraseña en texto claro (ej., una palabra simple o un número).
  4.  Introduje la contraseña en el sistema para obtener la bandera.

#### **- Solución**
`picoCTF{p0w3r_c4n_b3_c4p7ur3d_50d1a2}`

---

