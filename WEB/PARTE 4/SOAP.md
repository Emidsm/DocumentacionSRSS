- **Descripción del Reto:** El desafío implica la interacción con un servicio web que utiliza el protocolo **SOAP** (Simple Object Access Protocol). La bandera está oculta en los datos intercambiados con el servicio.
    
- **Procedimiento (Paso a Paso):**
    
    1. Identifiqué el _endpoint_ (URL de acceso) del servicio SOAP, a menudo terminando en `.asmx` o similar.
        
    2. Utilicé una herramienta como **`curl`** o **SoapUI** para interactuar con el servicio.
        
    3. Envié una solicitud SOAP al servidor. A menudo, esto requiere ver el WSDL (Web Services Description Language) para entender las funciones disponibles.
        
    4. Llamé a una de las funciones del servicio web, o modifiqué la solicitud SOAP, y la bandera fue devuelta en la respuesta XML.
        
- **La Bandera:** `picoCTF{s04p_1s_4_b1t_d1rty_f04e8a}`