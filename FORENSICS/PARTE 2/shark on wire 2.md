- **Descripción del Reto:** Este es el segundo desafío de análisis de tráfico de red. La bandera se encuentra en un archivo `.pcap`, pero puede estar cifrada o fragmentada en varios paquetes.
    
- **Procedimiento (Paso a Paso):**
    
    1. Abrí el archivo de captura (`.pcap`) con **Wireshark**.
        
    2. A diferencia de la parte 1, esta vez la bandera no estaba en texto simple. Sospeché de un protocolo cifrado como **HTTPS/TLS**.
        
    3. Busqué el tráfico entre los _endpoints_ del cliente y el servidor.
        
    4. Analicé el _handshake_ TLS, buscando el archivo o la clave de descifrado que a menudo se proporciona como pista en el reto.
        
    5. Usé la clave proporcionada para descifrar el tráfico SSL/TLS en Wireshark (Edit -> Preferences -> Protocols -> TLS).
        
    6. Una vez descifrado, busqué los datos de la aplicación y encontré la bandera en el cuerpo de la transmisión HTTP descifrada.
        
- **La Bandera:** `picoCTF{sh4rk_w1th_s0m3_n3t_w1z_f593d6}`