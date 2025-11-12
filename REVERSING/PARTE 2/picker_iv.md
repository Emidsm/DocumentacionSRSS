### **Picker IV**

#### **- Descripción del reto**
* El desafío final de la serie Picker, que requiere una explotación avanzada combinando una vulnerabilidad de **escritura** con **Return-Oriented Programming (ROP)** o **Return-to-Libc (ret2libc)**.

#### **- Procedimiento**
* **Identificación del problema:** El *exploit* requiere la ejecución de comandos del sistema operativo (`/bin/sh`) a través de la manipulación de la librería del sistema (`libc`).
* **Herramientas usadas:** *Script* de Python (`pwntools`), *leaks* de memoria.
* **Pasos para la solución:**
  1.  **Filtrado (Leak):** Utilicé una vulnerabilidad para **filtrar** una dirección de memoria de `libc` (la librería del sistema).
  2.  **Cálculo de Base:** Con el *leak*, calculé la dirección base de `libc`.
  3.  **Cadena ROP:** Construí una cadena **ROP** para llamar a la función `system()` con el argumento `/bin/sh`.
  4.  Sobrescribí la dirección de retorno para iniciar la cadena ROP y obtener un *shell* interactivo desde el cual leer la bandera.

#### **- Solución**
`picoCTF{p1ck3r_iv_r3t_t0_w1n_92c1b2}`
