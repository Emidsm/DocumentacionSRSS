### **EVEN RSA CAN BE BROKEN???**

#### **- Descripción del reto**
* Un desafío de RSA que explota un **fallo de implementación** o una debilidad de clave, a menudo porque los primos $p$ y $q$ son demasiado pequeños o tienen una relación matemática que permite una factorización rápida.

#### **- Procedimiento**
* **Identificación del problema:** Se proporcionaron los parámetros RSA ($n$, $e$, $c$), y se asumió que $n$ era factorizable debido al título del reto.
* **Herramientas usadas:** Factorización de Fermat o FactorDB (para factorizar $n$), Python (para descifrar).
* **Pasos para la solución:**
  1.  Identifiqué el módulo $n$.
  2.  Utilicé **FactorDB** para intentar encontrar los factores primos $p$ y $q$ de $n$. Dado que el reto implica un fallo, la factorización fue rápida.
  3.  Con $p$ y $q$, calculé $\phi(n) = (p-1) \times (q-1)$.
  4.  Calculé la clave privada $d = e^{-1} \pmod{\phi(n)}$.
  5.  Descifré el mensaje: $m = c^d \pmod{n}$, y convertí $m$ a ASCII.

#### **- Solución**
`picoCTF{w34k_R54_1s_n0_g0_f3a1d9}`

---

