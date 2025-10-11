- **Descripción del Reto:** El desafío implica la explotación de una tienda virtual que utiliza una lógica de precios defectuosa, lo que permite comprar la bandera sin tener suficiente "dinero".
    
- **Procedimiento (Paso a Paso):**
    
    1. El programa mostró mi saldo inicial y el precio de varios artículos, incluida la bandera (que era demasiado cara).
        
    2. Busqué una **opción de _overflow_** (desbordamiento) o una opción de "vender" con un precio negativo o muy alto.
        
    3. Encontré un artículo con un precio que, si lo compraba o vendía, causaba un desbordamiento del entero, resultando en un saldo positivo o negativo muy alto.
        
    4. Aumenté mi saldo con la explotación y luego compré la bandera.
        
- La Bandera:
    
    picoCTF{sh0p_t1ll_y0u_dr0p_4b3c2d}