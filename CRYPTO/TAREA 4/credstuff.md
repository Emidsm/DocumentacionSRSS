### **credstuff**

#### **- Descripción del reto**
* La bandera está oculta en una lista de **credenciales** (nombres de usuario y contraseñas) que han sido expuestas o filtradas en un archivo.

#### **- Procedimiento**
* **Identificación del problema:** Se proporcionó un archivo de texto que contenía una larga lista de pares de `username:password`.
* **Herramientas usadas:** Comandos de Linux (`cat`, `grep`), editor de texto.
* **Pasos para la solución:**
  1.  Utilicé el comando `cat` para ver el contenido del archivo.
  2.  Filté la lista de credenciales usando **`grep`** para buscar palabras clave como `flag`, `admin`, `picoCTF` o un nombre de usuario que destacara. El comando fue `cat creds.txt | grep -i flag`.
  3.  Encontré una entrada, a menudo con el nombre de usuario `flag` o `admin`, y su contraseña era la bandera.

#### **- Solución**
`picoCTF{cR3D5_4r3_345y_t0_f1Nd_e2c1b2}`

---

