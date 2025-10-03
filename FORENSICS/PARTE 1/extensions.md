- **Descripción del Reto:** La bandera se encuentra en un archivo que tiene una extensión incorrecta o engañosa. El objetivo es identificar el tipo de archivo real y abrirlo correctamente.
    
- **Procedimiento (Paso a Paso):**
    
    1. Descargué el archivo con la extensión incorrecta (por ejemplo, `file.jpg`).
        
    2. Utilicé el comando de Linux **`file`** para determinar el tipo de archivo real. El comando fue `file [nombre_del_archivo]`. Por ejemplo, me indicó que el archivo era en realidad un `.zip`.
        
    3. Cambié la extensión del archivo al tipo correcto (por ejemplo, `mv file.jpg file.zip`).
        
    4. Descomprimí o abrí el archivo para acceder a su contenido, que era un archivo de texto con la bandera.
        
- **La Bandera:** `picoCTF{f1l3_3xt3ns10n5_4r3_m34n_93a7c5}`