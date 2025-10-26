### **Mind your Ps and Qs - s3.py**

#### **- Descripción del reto**
* La bandera está cifrada con RSA, donde los factores primos $p$ y $q$ son muy cercanos entre sí. Esta condición hace que $n$ sea vulnerable al ataque de **Factorización de Fermat**.

#### **- Procedimiento**
* **Identificación del problema:** Se proporcionaron $n$ y $e$. El desafío requería un método de factorización especializado debido a la relación entre $p$ y $q$.
* **Herramientas usadas:** *Script* de Python (para Factorización de Fermat).
* **Pasos para la solución:**
  1.  **Ataque de Fermat:** La factorización de Fermat es eficiente cuando $p$ y $q$ están cerca. Un *script* de Python se utilizó para iterar hasta encontrar un valor $a$ tal que $a^2 = n + b^2$ (donde $a^2$ y $b^2$ son cuadrados perfectos).
  2.  **Encontrar $p$ y $q$:** Una vez encontrado $a$ y $b$, se calculó $p = a - b$ y $q = a + b$.
  3.  **Calcular $d$ y Descifrar:** Con $p$ y $q$, se procedió como en el RSA estándar (calcular $\phi(n)$, encontrar $d$, y descifrar $c$).

#### **- Solución**
`picoCTF{f3rm4t_4774ck_d3t3ct3d_7d1c2f}`

---

