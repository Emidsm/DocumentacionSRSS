### **b00tl3gRSA2 - s4.py**

#### **- Descripción del reto**
* El desafío implica un ataque de **exponente bajo ($e$)** de RSA (generalmente $e=3$), donde el texto cifrado $c$ es muy pequeño, permitiendo un descifrado rápido sin factorizar $n$.

#### **- Procedimiento**
* **Identificación del problema:** Se proporcionó $c$, $e$ (con $e=3$) y $n$. El valor de $c$ era pequeño, lo que sugiere que $c = m^e < n$.
* **Herramientas usadas:** Python (para raíz $e$-ésima).
* **Pasos para la solución:**
  1.  **Comprobación:** Verifiqué si $c < n$. Debido a que $e=3$ y $c$ era pequeño, se cumplía la condición $m^3 < n$.
  2.  **Descifrado con Raíz Cúbica:** Dado que $c = m^3 \pmod{n}$, y $m^3 < n$, el módulo no tiene efecto, por lo que $c = m^3$.
  3.  **Recuperar $m$:** Calculé la raíz cúbica de $c$: $m = \sqrt[3]{c}$.
  4.  **Conversión:** Convertí el resultado decimal $m$ a ASCII para obtener la bandera.

#### **- Solución**
`picoCTF{sm4ll_3xp0n3nt_l34ds_t0_fl4g_8a9b3c}`

---

