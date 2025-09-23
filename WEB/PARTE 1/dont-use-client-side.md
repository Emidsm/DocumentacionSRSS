
- **Descripción del Reto:** La bandera está protegida por una validación del lado del cliente. El objetivo es omitir esta validación para obtener acceso a la bandera.
    
- **Procedimiento (Paso a Paso):**
    
    1. Abrí la página y vi un formulario de entrada. Al inspeccionar el código, vi que la contraseña requerida estaba codificada en el archivo JavaScript.
        
    2. Copé la contraseña del código fuente.
        
    3. A pesar de que el formulario mostraba un error si la contraseña era incorrecta, pude simplemente enviarla sin usar la interfaz, o editar el HTML del formulario para eliminar la restricción.
        
    4. Al enviar la contraseña correcta, el servidor me dio la bandera.
        
- **La Bandera:** `picoCTF{cl1ent_s1d3_1s_b4d_c020d5}`