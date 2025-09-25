- **Descripción del Reto:** La bandera se encuentra en una base de datos, y el reto consiste en explotar una vulnerabilidad de **inyección SQL** para saltarse el formulario de inicio de sesión y acceder a los datos.
    
- **Procedimiento (Paso a Paso):**
    
    1. Abrí el formulario de inicio de sesión de la página web.
        
    2. En el campo de "username", ingresé `' OR 1=1 --`.
        
    3. En el campo de "password", dejé el campo vacío.
        
    4. El código SQL del servidor se convirtió en algo como `SELECT * FROM users WHERE username = '' OR 1=1 --' AND password = ''`.
        
    5. La expresión `1=1` siempre es verdadera, y los guiones `--` comentan el resto de la consulta, por lo que el servidor me autenticó como un usuario válido, lo que me dio acceso a una página con la bandera.
        
- **La Bandera:** `picoCTF{sQL_1nj3ct10n_3f2b45}`