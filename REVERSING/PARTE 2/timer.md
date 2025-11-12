### **timer**

#### **- Descripción del reto**
* El reto implica un programa binario que requiere la entrada del usuario en un **período de tiempo extremadamente corto** antes de que un *timer* lo termine.

#### **- Procedimiento**
* **Identificación del problema:** El programa utiliza la función `sleep()` o `alarm()` para limitar el tiempo de respuesta, lo que requiere automatización.
* **Herramientas usadas:** *Script* de Python (con **`pwntools`**).
* **Pasos para la solución:**
  1.  Analicé el código para confirmar la función de retardo.
  2.  Escribí un **script de automatización** en Python.
  3.  El *script* se conectó al programa a través de tuberías (`p.sendline()`) y envió la contraseña o la entrada requerida inmediatamente (casi al mismo tiempo que el servidor la solicitó), superando el límite de tiempo.

#### **- Solución**
`picoCTF{t1m3_1s_n0w_50d1a2}`

