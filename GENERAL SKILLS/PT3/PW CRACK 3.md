
### - Descripción del reto

Can you crack the password to get the flag? Download the password checker [here](https://artifacts.picoctf.net/c/17/level3.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/17/level3.flag.txt.enc) and the [hash](https://artifacts.picoctf.net/c/17/level3.hash.bin) in the same directory too. There are 7 potential passwords with 1 being correct. You can find these by examining the password checker script.
### - Procedimiento
Primero intenté meterle los archivos ya hasheados desde la entrada del teclado, lo cual estaba mal porque volvía a hashearlos y no valían nada, pero entonces vi que en una parte del código indicaba las 7 posibles contraseñas, entonces lo único que hice fue que no solicite entrada al usuario y que usando un ciclo, intente con las 7 contraseñas y entonces imprima la entrada.
### - Post mortem

Leer el código principal primero.
### - Solución

no la guardé :b