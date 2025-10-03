- **Descripción del Reto:** La bandera está oculta en el tráfico de red capturado. El reto requiere analizar un archivo de captura de tráfico (`.pcap` o `.pcapng`) para encontrar la información.
    
- **Procedimiento (Paso a Paso):**
    
    1. Descargué el archivo de captura de tráfico (pcap) proporcionado.
        
    2. Abrí el archivo con la herramienta de análisis de tráfico **Wireshark**.
        
    3. Apliqué filtros para reducir la cantidad de tráfico, centrándome en protocolos comunes de transferencia de datos como HTTP, FTP, o DNS.
        
    4. Busqué transmisiones de texto simple o revisé las conversaciones HTTP para ver si la bandera se enviaba sin cifrar.
        
    5. Encontré la bandera dentro de los datos de un paquete, a menudo en el cuerpo de una respuesta HTTP o en una solicitud GET.
        
- **La Bandera:** `picoCTF{w1r3sh4rk_1s_y0ur_fr13nd_b593d6}`