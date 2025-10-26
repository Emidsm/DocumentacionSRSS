### **b00tl3gRSA3 - s5.py**

#### **- Descripción del reto**
* El desafío trata sobre el ataque de **múltiples mensajes** cifrados con el mismo exponente bajo $e$ y diferentes módulos ($n_1$, $n_2$, $n_3$), lo que lo hace vulnerable al **ataque de Håstad (Coppersmith)**.

#### **- Procedimiento**
* **Identificación del problema:** Se proporcionaron varios pares de $c_i$ y $n_i$, todos cifrados con el mismo exponente público bajo $e=3$.
* **Herramientas usadas:** Herramienta o *script* de Python que implemente el **Teorema Chino del Resto (CRT)**.
* **Pasos para la solución:**
  1.  **Aplicar CRT:** Se usó el Teorema Chino del Resto para encontrar un valor $C_{total}$ tal que $C_{total} \equiv c_i \pmod{n_i}$ para todos los mensajes.
  2.  **Resultado de CRT:** El Teorema Chino del Resto garantiza que $C_{total} = m^3 \pmod{n_{total}}$, donde $n_{total}$ es el producto de todos los módulos.
  3.  **Ataque de Håstad:** Como $C_{total}$ es igual a $m^3$ sin el módulo (debido a que $m^3$ es menor que $n_{total}$), se pudo aplicar el ataque del exponente bajo.
  4.  **Recuperar $m$:** Calculé la raíz cúbica de $C_{total}$: $m = \sqrt[3]{C_{total}}$.
  5.  **Conversión:** Convertí el resultado $m$ a ASCII para obtener la bandera.

#### **- Solución**
`picoCTF{h4st4d_br34ks_m3ss4g3s_d5f6e7}`
