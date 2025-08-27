### - Descripción del reto

Our flag printing service has started glitching!
Additional details will be available after launching your challenge instance.
### - Procedimiento
Ejecuté el comando de netcat en el webshell, lo que me arrojó esta cadena
'picoCTF{gl17ch_m3_n07_' + chr(0x62) + chr(0x64) + chr(0x61) + chr(0x36) + chr(0x38) + chr(0x66) + chr(0x37) + chr(0x35) + '}'

logré identificar caractéres en hexadecimal https://www.rapidtables.com/convert/number/hex-to-ascii.html, por lo que me fui al conversor de hex to ASCII/UTF-8, los carácteres cifrados son: bda68f75, por lo que reemplazando en la cadena, quedaría como se ve en la solución
### - Solución

picoCTF{gl17ch_m3_n07_bda68f75}
picoCTF{gl17ch_m3_n07_bda68f75}
### - NOTAS
Era más rápido abrir python y ejecutar un print
