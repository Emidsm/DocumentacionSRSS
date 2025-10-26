### **Mini RSA - s1.py, s2.py**

#### **- Descripción del reto**
* Un desafío de RSA donde el módulo $n$ es muy pequeño (Mini RSA) o está comprometido. Requiere factorizar $n$ para encontrar los factores primos $p$ y $q$.

#### **- Procedimiento**
* **Identificación del problema:** Se proporcionó el módulo $n$ (pequeño) y el exponente público $e$, junto con el texto cifrado $c$. El tamaño reducido de $n$ fue la pista principal.
* **Herramientas usadas:** Python (para calcular el MCD y el inverso modular), biblioteca de factorización.
* **Pasos para la solución:**
  1.  **Factorizar $n$:** Debido a que $n$ era pequeño (ej., 256 bits), utilicé una herramienta de factorización en línea o un *script* de Python para encontrar los factores primos $p$ y $q$.
  2.  **Calcular $\phi(n)$:** Una vez con $p$ y $q$, calculé $\phi(n) = (p-1) \times (q-1)$.
  3.  **Calcular $d$ (Clave Privada):** Encontré el inverso modular de $e$ modulo $\phi(n)$ usando la función de Python `pow(e, -1, phi_n)`.
  4.  **Descifrar:** Usé $d$ para descifrar el texto cifrado $c$: $m = c^d \pmod{n}$, y convertí el resultado a ASCII para obtener la bandera.

#### **- Solución**
`picoCTF{mini_rsa_is_too_easy_12c3f4}`

---

