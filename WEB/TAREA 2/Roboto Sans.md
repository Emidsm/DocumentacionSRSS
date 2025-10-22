
- **Descripción del Reto:** El nombre sugiere que la bandera está oculta en los archivos de un sitio web, haciendo referencia a fuentes (Roboto Sans) o recursos estáticos que se cargan en segundo plano.
    
- **Procedimiento (Paso a Paso):**
    
    1. Abrí la página web y la herramienta de desarrollador en la pestaña **"Network"** (Red).
        
    2. Recargué la página para ver todos los archivos que se cargaban (imágenes, CSS, fuentes).
        
    3. Busqué archivos con nombres inusuales o extensiones que no eran de fuente.
        
    4. Encontré un archivo de fuente (`.ttf` o `.woff`) que, al ser analizado con `strings` o simplemente al intentar descargarlo, contenía un comentario o un metadato con la bandera.
        
- La Bandera:
    
    picoCTF{r0b0t0_s4n5_c4n_h1d3_f1les_3f2b45}
    
