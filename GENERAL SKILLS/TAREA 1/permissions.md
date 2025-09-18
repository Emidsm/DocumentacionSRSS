
### **1. Descripción del Reto**
> *El objetivo era encontrar la bandera en un sistema de archivos de Linux, donde los permisos de un archivo o directorio impedían el acceso directo.*

### **2. Procedimiento (Paso a Paso)**
* **Identificación del problema:** La terminal me decía "Permission denied" al intentar listar un directorio. Esto me indicó que la solución estaba en entender los permisos.
* **Herramientas usadas:** `ls -l`, `cd`, `cat`.
* **Pasos para la solución:**
  1.  Utilicé `ls -l` para listar todos los archivos y carpetas, revelando los permisos de cada uno.
  2.  Noté que un directorio llamado `flag` tenía permisos de ejecución para mi usuario, pero no de lectura.
  3.  Usé `cd flag` para entrar a la carpeta. Una vez dentro, pude usar `ls -l` nuevamente para ver un archivo llamado `the_flag.txt`.
  4.  Finalmente, usé `cat the_flag.txt` para leer el contenido y obtener la bandera.

### **3. La Bandera**
`picoCTF{f1l3_p3rm1ss10n5_4r3_1mp0rt4nt_9a7524}`