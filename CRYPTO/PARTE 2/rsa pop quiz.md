#### **- Descripción del reto**

	Class, take your seats! It's PRIME-time for a quiz... 
	`nc jupiter.challenges.picoctf.org 1981`

- Este es un desafío de criptografía que requiere conectarse a un servidor para responder una serie de **8 preguntas de cálculo** sobre los conceptos fundamentales del algoritmo **RSA** ($n$, $p$, $q$, $\phi(n)$, $e$, $d$).

#### **- Procedimiento**

- **Identificación del problema:** El reto se resuelve interactuando con un servidor vía `netcat` (`nc`) y utilizando un script de Python para realizar los cálculos RSA necesarios en tiempo real.
    
- **Herramientas usadas:** Terminal (con `netcat`), script de Python (para cálculos modulares rápidos).
    
- **Pasos para la solución (Desglosados por Operación):**
    
    1. **Conexión:** Me conecté al servidor con `nc [IP] [puerto]`.
        
    2. **Calcular $n$:** Si me dieron $p$ y $q$, usé Python para calcular el módulo: $n = p \times q$.
        
    3. **Calcular $q$ (o $p$):** Si me dieron $n$ y $p$, usé Python para dividir: $q = n / p$.
        
    4. **Feasibility (Factorización):** Cuando me pidieron factorizar un $n$ muy grande, respondí **`N`** (No) ya que no es computacionalmente factible.
        
    5. **Calcular $\phi(n)$:** Si me dieron $p$ y $q$, usé Python para calcular $\phi(n) = (p - 1) \times (q - 1)$.
        
    6. **Calcular $c$ (Texto Cifrado):** Si me dieron $m$, $e$ y $n$, usé la función de Python `pow(m, e, n)`.
        
    7. **Calcular $d$ (Clave Privada):** Si me dieron $p$, $q$ y $e$, primero calculé $\phi(n)$ y luego el inverso modular con `pow(e, -1, phi_n)`.
        
    8. **Calcular $m$ (Texto Plano) final:** Si me dieron $c$, $d$ y $n$, usé `pow(c, d, n)`. El resultado decimal lo convertí a hexadecimal y luego a **ASCII** para obtener la bandera.
        

#### **- Flag**

`picoCTF{wA8_th4t$_ill3aGal..ode01e4bb}`