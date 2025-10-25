Ph4nt0m 1ntrud3r

- Descripción del reto

Ph4nt0m 1ntrud3r

- Descripción del reto

    El desafío se enfoca en el análisis forense de un archivo de red o un sistema, con la pista de un "intruso fantasma," lo que sugiere que la actividad de la bandera fue eliminada o está muy bien escondida.

- Procedimiento

    Identificación del problema: Se proporcionó un archivo de tráfico de red (pcap) o una imagen de disco con actividad eliminada.

    Herramientas usadas: Wireshark (o Volatility), filtros de tráfico, análisis de logs.

    Pasos para la solución:

        Abrí el archivo pcap en Wireshark.

        Busqué tráfico que pudiera indicar la eliminación o actividad sospechosa (ej., tráfico DNS a un servidor de Command and Control, o peticiones HTTP inusuales).

        Utilicé un filtro de Wireshark para buscar tráfico oculto o sin protocolo (tráfico fantasma).

        Encontré un paquete con datos codificados (ej., Base64) que contenían la bandera.

- Solución

picoCTF{ph4nt0m_p4ck3ts_4r3_n0_m4tCh_b593d6}
